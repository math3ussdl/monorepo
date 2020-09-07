# Merge Repo (Convert to MonoRepo)

Follow the steps bellow to setup a project:

1) After you create the root directory of your project, follow the commands below:

  ```console
  admin@localhost:~$ git init
  Initialized empty Git repository in [...]/.git
  ```

  ```console
  admin@localhost:~$ git remote add [name_of_the_repo / ex: server] [link_repo]
  ```

  OBS: Repeat the previous step by project that you want to join!


2) Get all projects with Git's fetch command

  ```console
  admin@localhost:~$ git fetch --all --no-tags
  ```


3) Building your MonoRepo

  3.1) Download MonoRepo Tools

    ```console
    admin@localhost:~$ git clone https://github.com/shopsys/monorepo-tools [destination directory]
    ```

  3.2) Execute the MonoRepo Tools' command to building your MonoRepo project passing the project folders and your destination path!

    ```console
    admin@localhost:~$ [path_to_monorepo-tools]/monorepo_build.sh server:packages/server mobile:packages/mobile
    ```
