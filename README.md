# cloud-config-pivotal-cloud-foundry


Create a configuration file cfg.json

{  
  "git":{  
    "uri":"https://github.com/saagarwal-pivotal/config-server.git",
    "label":"master",
    "searchPaths":"master"
  }
}
Register the config-server

$ cf create-service -c cfg.json p-config-server trial my-config-server