# Java Quick Bot

JQB is an easy to use discord bot maker with a built in basic command system.

## Installation

The API is provided in jar form on github.

```html
https://github.com/KyonDevelopment/JQB/tree/master/
```

## Usage

```java
new Bot()
	.setPrefix("!")
	.addCommand(new Command("test") {
		@Override
		public void onCommand(Member member, Message message, String aliasUsed, String[] args) {
			message.getChannel().sendMessage("this works!").queue();
		}
	})
	.build("Token");
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)