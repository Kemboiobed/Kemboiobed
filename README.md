{
  "name": "𝐉𝐎𝐑𝐃𝐀𝐍-𝐉𝐎𝐄𝐋𝐒𝐓𝐀𝐑 🤖",
  "description": "Hi there, I am 𝐉𝐎𝐑𝐃𝐀𝐍-𝐉𝐎𝐄𝐋𝐒𝐓𝐀𝐑 🤖  Whatsapp multifunctional bot built in NodeJs by JORDAN to make experience better.\n\t Incase of Any Problem Whatsapp me on: +2349054039891",
  "logo": "https://telegra.ph/file/473b1a392c20882309874.jpg",
  "keywords": ["whatsappbot", "suhailMd", "suhail Md bot", "Suhail-Md", "SuhailMdWhatsaooBot", "SuhailWaBot","SuhailMD","Suhail Md Whatsapp Bot","multi device"],
  "success_url": "/JORDAN-JOELSTAR/",
  "app_url": "/JORDAN-JOELSTAR/",

  "env": {
    "OWNER_NAME": {
      "description": "Name of Bot Owner",    
      "value": "𝐉𝐎𝐑𝐃𝐀𝐍 𝐉𝐎𝐄𝐋𝐒𝐓𝐀𝐑",
      "required" :true
    },   

    "WELCOME": {
      "description": "put 'false' or 'true' to enable & disable automatic group WELCOME ",
      "value": "false",
      "required" :true
    },

    "GOODBYE": {
      "description": "put 'false' or 'true' to enable & disable automatic group GOODBYE ",
      "value": "false",
      "required" :true
    },
    "BOT_NAME": {
      "description": " NAME FOR BOT",
      "required" :true,    
      "value": "𝐉𝐎𝐑𝐃𝐀𝐍-𝐉𝐎𝐄𝐋𝐒𝐓𝐀𝐑 🤖"
    }, 
    "IMAGE": {
      "description": "Image for bot",
      "required" :true,    
      "value": "https://telegra.ph/file/04e1e12ab2d93f3e7dae4.jpg"
    }, 
    "TZ": {
      "description": "Put TIME_ZONE according to your location",
      "required" :true,    
      "value": "Africa/Lagos"
    },  
    "FLUSH": {
      "description": " Make it 'true' if bot connected but not responding (After deployement!)",
      "required" :true,    
      "value": "true"
    }, 
    "WARN_COUNT": {
      "description": " Warn count for users to kick/block when warn limit exceed!",
      "required" :true,    
      "value": "2"
    }, 
    "READ_COMMAND": {
      "description": " Read bot cmds",
      "required" :true,    
      "value": "true"
    }, 
    "AUTO_SAVE_STATUS": {
      "description": " Auto save whatsapp status", 
      "required" :true,   
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
      "description": "Fill the value: 'unavailable'(for nothing) | 'available'(for alwaysonline) | 'composing'(for always online and virtual typing) | 'recording'(for always online and virtual recording audio) | 'paused' ",
      "required" :true,
      "value": "available"
    },
    "AUTO_READ_STATUS": {
      "description": "Fill the value true if you want bot to automatically view your Statuses.",
      "required" :true,
      "value": "true"
    }, 
    "MSGS_IN_LOG": {
      "description": "Fill the value true if you want to see Messages in Console.",
      "required" :true,
      "value": "false"
    },
    "READ_MESSAGE": {
      "description": "Fill the value true if you want bot to read all messages that is auto blue ticks.",
      "required" :true,
      "value": "false"
    },
    "DISABLE_PM": {
      "description": "Disable bot in pm, Take it false if you wanna run bot in your pm (if MODE is Public)",
      "value": "true",
      "required" :true
    },
    "PREFIX": {
      "description": "Enter your desired prefix for bot.",
      "required" :true,
      "value": "."
    },
    "OWNER_NUMBER": {
      "description": "The phone numbers of the users who you want to be admin for the bot (should be in international format without + and multiple numbers must be separated by a comma \",\")",
      "required" :true,
      "value": "2349054039891, 2347061138624"
    },
    "SESSION_ID": {
      "description": "put your SESSION_ID here.",
      "required" :true,
      "value": ""

    },
    "OPENAI_API_KEY": {
      "description": "put your OPENAI api key here.Get it from beta.openai.com ",
      "value": "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",
      "required" :true
    }, 
    "ELEVENLAB_API_KEY": {
      "description": "Put your ElevenLab api key here for Aitts. Watch tutorial from https://youtu.be/HCDcdPtkwg4 ",
      "value": "b83709a7a0691e09fbe13db39068056a",
      "required" :true
    }, 
    "REMOVE_BG_KEY": {
      "description": "put your REMOVE BG KEY here.Get it from removeBg.com ",
      "value": "diVYfA5PJpwMSDrMCj2BYbnc",
      "required" :true
    },
    "MODE": {
      "description": "Worktype of your bot. Use public or private, if it is private then only bot number can use it. If public then everyone can use it.",
      "required" :true,
      "value": "private"
    },
    "PACK_NAME": {
      "description": "Put Sticker Pack_Name.",
      "value": "𝙹𝙾𝚁𝙳𝙰𝙽-𝙹𝙾𝙴𝙻𝚂𝚃𝙰𝚁",
      "required": true 
    },
    "PACK_AUTHER": {
      "description": "Put Sticker Author_Name.",
      "value": "𝙹𝙾𝚁𝙳𝙰𝙽-𝙹𝙾𝙴𝙻𝚂𝚃𝙰𝚁🤖",
      "required": true 
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