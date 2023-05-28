# 🦀 MeterFeeder 🦀
This repository is a rust based (safe-ish) wrapper around the C++ based [LibMeterFeeder](https://github.com/TheRandonauts/MeterFeeder). This should make it easier to `MED_DEVICES` from rust based projects. Oh and it only work on linux rn.



### Compiling
```
$ cargo --release build
```

### Install

We need to have meterfeeders so file in the path for the library to use it. PR's appreciated if you can work around that.
```
$ sudo cp ./libmeterfeed.so /usr/lib 
```


#### Tests

Run the test cases, you need to specficy the current directory into the path so the `SO` file is available
##### Normal
```
$ LD_LIBRARY_PATH=. cargo test
```

##### With outputs
```
$ LD_LIBRARY_PATH=. cargo test -- --nocapture
```


## Contributing

We don't have a very specific contributing guidelines right now so just feel free to do the following. Contributors are always appreciated!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request


<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.MD` for more information.