\# v2ray-cloudfoundry

push v2ray on ibm cloudfoundry

  

english:

  

//open ibm shell

  

`git clone https://github.com/wenxhwork/coxray.git`

`cd coxray/coxray`

`chmod +x *`

//you can edit config.json as you want

`cd ..`

  

//edit manifest.yml

applications:

\- path: .

  name: GetStartedGo//change this name to your cloudfoundry name

  random-route: true

  memory: 128M//change memory to 64M,128M,256M

  

`ibmcloud target --cf`

`ibmcloud cf push`

  

//waiting cloudfoundry restart success!

