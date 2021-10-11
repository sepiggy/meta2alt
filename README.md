cmake -B build -DCMAKE_BUILD_TYPE=Release

make -C build

- JOB: "intercept -g $DEVNODE | caps2esc -m 1 | meta2alt | uinput -d $DEVNODE"
  DEVICE:
      LINK: /dev/input/by-path/platform-i8042-serio-0-event-kbd

