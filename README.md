# MMM-Inspirational-Quotes
![Demo1](https://i.imgur.com/HTIuR5P.png)
Need to get a bit more inspired in the morning? Well then this probably isn't the module for you. However, if you want to have a quick laugh at a machine trying to emulate the structure of an inspirational quote? Now we're getting somewhere.

MMM-Inspirational-Quotes uses [InspiroBot](https://inspirobot.me/) for the backend generation. Be careful, it you visit that website, you may never stop clicking generate.

## Installation
Navigate to the modules folder of your Magic Mirror installation.
```bash
cd ~/MagicMirror/modules
```

Clone the repository.
```bash
git clone https://github.com/Veldrovive/MMM-Inspirational-Quotes.git
```

## Usage
```js
  modules: [
    ...
    {
      module: "MMM-Inspirational-Quotes",
      position: "top_left",
      config: {
        update_interval: 5000 // How often to switch the quote in milliseconds. By default, this is 0 meaning never change
        transition_interval: 2000 // The transition time between one image and the next
        size: "500px" // The size of the image
      }
    }
    ...
  ]
```

## Configuration
Option|Description
------|-----------
`update_interval`|The number of milliseconds between changing the quote. If this is not set, the quote will never change. <br/>**Expected Value Type:** `Integer`
`transition_interval`|The number of milliseconds it takes for the transition between one image and another the happen. <br/>**Expected Value Type:** `Integer`
`size`|The size of the image. <br/>**Expected Value Type:** `String (Valid css value)`

## Integration with other modules
Any module can send a notification to `NEXT_QUOTE`.



Ok, here's one more example.
![demo2](https://i.imgur.com/QIUdDh0.png)
