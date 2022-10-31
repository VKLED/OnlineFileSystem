# server needs to run before client

# config 
framework.view.fileManagerPage: line 430, split()

# First week
backend: login/signup/changeAccountSettings/logout
{
    method: run and debug
    file: {
        src/server/tests/ServerMain.java, 
        src/client/tests/ClientMain.java
    }
}
frontend: login/signup page
{
    method: run and debug
    file: {
        src/server/tests/ServerMain.java, 
        src/framework/view/fileStorage.java
    }
}

# Second week:
missions:{
    create/update/delete file/folder,
    upload file/folder,
    share files
}
run and debug: {
    src/server/tests/ServerMain.java,
    src/framework/view/fileStorage.java
}

# Third week:
mission: file concurrent editing

run/debug: {
    src/server/tests/ServerMain.java, 
    src/framework/view/fileStorage.java
}
