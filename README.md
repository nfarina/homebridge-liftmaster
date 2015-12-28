
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
