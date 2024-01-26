# OBR: Autonomous Unity/ROS2 Workspace

Repo containing the workspace structure


# Setup

### Step-by-step

1. Install vcstool (usually also available through package manager as python-vcstool)
    ```
    pip3 install --user vcstool
    ```
    ```
    pip3 install python3-vcstool
    ```
2. Clone this branch
    ```
    git clone git@github.com:Look-No-Hands-Simulator/unityros-ws.git && cd unityros-ws
    ```
4. Import set of repositories
    ```
    vcs import src < ursim.yaml
    ```

# Usage

### Update repositories
```
vcs pull src < ursim.yaml
```

### Build everything
```
colcon build --symlink-install
```

### Build one package
```
colcon build --symlink-install --packages-up-to <package>
```
> `--packages-select` if you don't want to reinstall dependencies

### Blacklist package
Blacklist a package from being built by colcon by creating a `COLCON_IGNORE` file in the specific repo
```
touch src/team_name/package_name/COLCON_IGNORE
```
> this file should already be part of the .gitignore for the repo

# Copy & paste
~~~

~~~

# Install
Unity
ROS2 foxy
Python3

