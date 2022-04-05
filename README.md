# Sakura Client
![GitHub repo size](https://img.shields.io/github/repo-size/demonicat/sakura-client)
[![GitHub](https://img.shields.io/github/license/demonicat/sakura-client)](https://github.com/demonicat/sakura-client/blob/master/LICENSE)


### Based on [mehah/otclient](https://github.com/mehah/otclient) Rev: [3.490](https://github.com/mehah/otclient/tree/c4433f3dba1e2790038495ab056848e3344190ac)

### Compiling on Arch Linux
Install necessary deps:
```sh
sudo pacman -Syu base-devel git cmake boost physfs openssl lua51 glew libvorbis openal zlib libogg nlohmann-json protobuf --needed
```

Get the sources:
```sh
git clone git@github.com:demonicat/sakura-client.git
```

Regenerate protobuf files:
```sh
cd sakura-client/src/framework/protobuf/proto/
./generate.sh
cd ../../../../
```

Compile:
```sh
cmake . -B build
make -C build -j$(nproc)
./build/sakuraclient
```

### License

Otclient is made available under the MIT License, thus this means that you are free
to do whatever you want, commercial, non-commercial, closed or open.
