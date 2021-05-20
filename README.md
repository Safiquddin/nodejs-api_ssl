# nodejs-api
For Jenkins job
plugins should be installed are Nodejs Plugin,Publish over ssh plugin(for deploy to docker server)
manage jenkins>>global tool configuration setup nodejs:7 install automatically
on freestyle job
1.scm this git url
2.on build environment node & bin folder to path
3 on build section npm install
4. On build section choose execute command & send files over ssh
   give the credential of docker server on manage jenkins>Global configuraion
   exec command section 
   copy all neccessary files & directory from jenkins workspace to remote docker server
   execute the docker-compose build then docker-compose up -d
