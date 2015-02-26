# G13 Profiles

To be used with [ecraven's G13 userspace driver](https://github.com/ecraven/g13).

## Getting the userspace driver running

If you get the error `/dev/uinput doesn't grant write permissions`, be lazy and run `$ sudo chmod a+rw /dev/uinput` and try it again.

## Usage
Clone to whereever. Cat the profile you want to use to /tmp/g13-0. Play games.

You can also use this little script to select a profile if you have dmenu installed:

    cat ~/.g13/$(ls ~/.g13 | grep bind$ | dmenu -i -p 'Set G13 Profile') > /tmp/g13-0

Change the two `~/.g13` paths if you aren't using it in `~/.g13`.

I have this bound in i3 to $mod+Shift+g, works great.

## Profiles available

* Default `default.bind`, a copy of the default bindings when using Logitech's "Gaming" software on Windows.