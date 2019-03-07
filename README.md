# ScienceDBStarterPack

ScienceDB can be used for different collecting data projects. 
Each projects can have have it's own data sets, project specific code, etc. However, 
all these projects are based on the same package: ScienceDBStarterPack.

As long as project specific data is also stored on the GitHub, it was decided at least for now, 
to keep this data within different branches of the ScienceDBStarterPack project.    

To install your project, that is stored within `YOUR_BRANCH` branch, use the command below: 

```
git clone --recursive -b YOUR_BRANCH https://github.com/ScienceDb/ScienceDbStarterPack.git
```

After this command, all submodules will be initialized and updated automatically (updated to the current 
versions in their repositories??? - check this).


To create a new project based on this package please run the script:
```
./scripts/install.sh
```

You can run this project in development or in production modes. Just add 
`docker-compose.yml` symlink to the corresponding `*_dev.yml` or `*_srv.yml` file.
This way you can use `docker-compose` command without `-f` option.


*****
TODO: What about project-specific installations? How to make it more generic?
Which rules to adjust? 
