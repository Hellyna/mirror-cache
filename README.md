# mirror-cache

Preliminary poc of an nginx caching based apt mirror. Feedback welcome.

Currently, the related nginx configuration (`mirror.conf`) contains ros, ros2, and gazebo mirrors to test the capabilities of multi mirror path setups.

# Usage

`docker-compose up`

Then, edit the relevant files in `/etc/apt/sources.list` or `/etc/apt/sources.list.d/*` to refer to the new mirror using your private IP address. (ie, something like `http://192.168.x.x/ubuntu`).
