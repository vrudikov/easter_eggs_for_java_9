
### Idea

* example that patches a module with an updated class
* see the shell scripts for the mechanics of the command-line args etc

### Execution Steps

* initial module:
    * `./clean.sh` 
    * `./compile.sh`
    * `./run.sh`
        * observe output as defined in `UserServiceImpl` in main code-base [here](https://github.com/codetojoy/easter_eggs_for_java_9/blob/master/egg_09_Patch_Module/src/net.codetojoy/net/codetojoy/service/impl/UserServiceImpl.java)
* with patch:
    * `cd patch`
    * `./build_patch.sh`
    * `cd ..`
    * `./run_with_patch.sh`
        * observe output as defined in patched `UserServiceImpl` [here](https://github.com/codetojoy/easter_eggs_for_java_9/blob/master/egg_09_Patch_Module/patch/src/net.codetojoy/net/codetojoy/service/impl/UserServiceImpl.java)
