
# Important Notice

This plugin is rather old - it still Works For Me™ so I haven't hacked on it much. If you are having trouble with it, I recommend checking out the newer [`homebridge-liftmaster2`](https://github.com/luisiam/homebridge-liftmaster2) by [luisiam](https://github.com/luisiam).

# LiftMaster Plugin

Example config.json:

    {
      "accessories": [
        {
          "accessory": "LiftMaster",
          "name": "Garage Door",
          "username": "your@email.com",
          "password": "your_password"
        }
      ]
    }

If you have multiple garage doors connected to your LiftMaster account, the plugin will print out an error followed by the multiple device IDs it found. You'll need to use these IDs to enter your doors as separate accessories:

    {
      "accessories": [
        {
          "accessory": "LiftMaster",
          "name": "Side Garage Door",
          "username": "your@email.com",
          "password": "your_password",
          "deviceID": "desired_device_id"
        }
      ]
    }
