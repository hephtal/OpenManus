if you want headless to work you need to you need to do some stuff

1. Install XQuartz: `brew install --cask xquartz`
2. Open XQuartz, go to Preferences -> Security, and check “Allow connections from network clients”
3. Go to Login Items in macos settings and make sure XQuartz is ticket and so is allowed in the background 
4. Restart your computer 
5. Start XQuartz with `xhost +localhost`
6. Then use `docker compose up`
7. then go to docker desktop and exec and run `python main.py`
8. Outputs of openmanus will be in the `workspace` directory


# resources 

https://www.oddbird.net/2022/11/30/headed-playwright-in-docker/
https://github.com/XQuartz/XQuartz/issues/295