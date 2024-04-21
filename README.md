{
  "name": "gifted-md@2.5.0",
  "description": "I am Gifted-Md Whatsapp MultiDevice Whatsapp Bot built in NodeJs to make experience better\n\t if Any Problem Whatsapp Me on: +254728782591",
  "logo": "https://telegra.ph/file/54efddccf41281ad7ec51.jpg",
  "keywords": ["whatsappbot", "giftedlMd", "gifted Md bot", "Gifted-Md", "GiftedMdWhatsaooBot", "GiftedWaBot","GiftedMD","Gifted Md Whatsapp Bot","multi device"],
  "success_url": "/",
  "app_url": "/qr/",

  "env": {
    "OWNER_NAME": {
      "description": "Name for Bot Owner",    
      "value": "Gifted Tech",
      "required" :true
    },   

    "WELCOME": {
      "description": "put 'false' or 'true' to enable & disable WELCOME ",
      "value": "false",
      "required" :false
    },

    "GOODBYE": {
      "description": "put 'false' or 'true' to enable & disable GOODBYE ",
      "value": "false",
      "required" :false
    },
    "BOT_NAME": {
      "description": " NAME FOR BOT",
      "required" :false,    
      "value": "ɢɪғᴛᴇᴅ-ᴍᴅ"
    }, 
    "USER_IMAGES": {
      "description": "Image for bot",
      "required" :false,    
      "value": "https://telegra.ph/file/54efddccf41281ad7ec51.jpg"
    }, 
    "TZ": {
      "description": "Put TIME_ZONE according to your location",
      "required" :false,    
      "value": "Africa/Nairobi"
    },  
    "FLUSH": {
      "description": " Make it 'true' if bot connected but not responed (After deployement!)",
      "required" :false,    
      "value": "true"
    },     
    "READ_COMMAND": {
      "description": " Read bot cmds",
      "required" :false,    
      "value": "true"
    },
    "WARN_COUNT": {
      "description": " Warn count for users to kick/block when warn limit exceed!",
      "required" :false,    
      "value": "5"
    },  
    "AUTO_SAVE_STATUS": {
      "description": " Auto save whatsapp status", 
      "required" :false,   
      "value": "false"
    }, 
    "HEROKU_API_KEY": {
      "description": "Put Your Heroku Api Key Here",
      "value": "",
      "required" :true 
    },   
    "HEROKU_APP_NAME": {
      "description": "Put Your Heroku App Name Here",
      "value": "",
    "required" :true
    }, 
    "WAPRESENCE": {
      "description": "Fill the value: 'unavailable'(for nothing) | 'available'(for alwaysonline) | 'composing'(for typing) | 'recording' | 'paused' ",
      "required" :false,
      "value": "available"
    },
    "AUTO_READ_STATUS": {
      "description": "Fill the value true if you want bot view your Statuses.",
      "required" :false,
      "value": "true"
    }, 
    "MSGS_IN_LOG": {
      "description": "Fill the value -true- if you want to see Messages in logs.",
      "required" :false,
      "value": "true"
    },
    "READ_MESSAGE": {
      "description": "Fill the value true if you want bot to read all messages.",
      "required" :false,
      "value": "false"
    },
    "DISABLE_PM": {
      "description": "Disable bot in pm, Take it false if you wanna run bot in your pm (if MODE is Public)",
      "value": "false",
      "required" :false
    },
    "PREFIX": {
      "description": "Enter your desired prefix for bot. you can set `all | . | .!*`",
      "value": "."
    },
    "OWNER_NUMBER": {
      "description": "The phone numbers of the users who you want to be admin for the bot (should be in international format without + and multiple numbers must be separated by a comma \",\")",
      "value": "254728782591,254762016957,254110853827,254728746852"
    },
    "SESSION_ID": {
      "description": "put your SESSION_ID here.",
      "value": ""

    },
    "OPENAI_API_KEY": {
      "description": "put your OPENAI api key here.Get it from beta.openai.com ",
      "value": "",
      "required" :false
    }, 
    "ELEVENLAB_API_KEY": {
      "description": "Put your ElevenLab api key here for Aitts. Watch tutorial from https://youtu.be/HCDcdPtkwg4 ",
      "value": "",
      "required" :false
    }, 
    "REMOVE_BG_KEY": {
      "description": "put your REMOVE BG KEY here.Get it from removeBg.com ",
      "value": "",
      "required" :false
    },
    "MODE": {
      "description": "Worktype of your bot. Use public or private, if it is private then only bot number can use it. If public then everyone can use it.",
      "value": "public"
    },
    "PACK_NAME": {
      "description": "Put Sticker Pack_Name.",
      "value": "Gifted Md",
      "required": false 
    },
    "PACK_AUTHER": {
      "description": "Put Sticker Author_Name.",
      "value": "Gifte Tech",
      "required": false 
    },
    "STACK": {
      "description": "STACK NAME ",
      "value": "container | heroku-22 | 4246315815290786|01|2026|717",
      "required": false 
    }
 }, 
  "addons": [
    {
      "plan": "heroku-postgresql:basic"
    } 
  ],
  "buildpacks": [
    { "url": "https://github.com/heroku/heroku-buildpack-nodejs#latest" },
    { "url": "https://github.com/carlosdommor/heroku-buildpack-ffmpeg-latest" }
  ],
  "formation": {
      "web": {
          "quantity": 1,
          "size": "standard-2x"
      }
  }
}