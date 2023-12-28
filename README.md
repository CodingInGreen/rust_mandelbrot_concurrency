# A Parallel Mandelbrot Set Plotter

This program plots the Mandelbrot set and writes it out as a PNG file. It uses Rust's concurrency primitives to distribute the work across eight threads.

This example is the multi-threaded version based on the Rayon crate in the "Concurrency" chapter of the Programming Rust Book.


It uses the Rayon library. Rayon provides a *parallel iterator* API that makes the code much simpler. It looks a lot like Rust code that uses plain old iterators. 

## Examples

### Mandelbrot Set
`cargo run mandel.png 1000x750 -1.20,0.35 -1,0.20`

### Sandy beach
`cargo run beach.png 1000x750 -0.99,0.50 -1,0.25`

### Zooming into the boundary near the main cardioid
`cargo run zoom.png 1000x750 -0.75,0.1 -0.74,0.11`

### Exploring the Seahorse Valley
`cargo run seahorse.png 1000x750 -0.746,0.095 -0.745,0.096`

### Complex plane regions with fine, filament-like structures
`cargo run filament.png 1000x750 -0.22,0.70 -0.21,0.71`

### Areas where the set has 'whisps' that are evocative of smoke tendrils
`cargo run whisps.png 1000x750 -1.5,0.02 -1.4,0.03`

### Structures being sucked into a black hole
`cargo run blackhole.png 1000x750 -0.748,0.1 -0.747,0.101`

## License

The example code in this directory and its subdirectories is licensed under the
terms of the MIT license. See [LICENSE-MIT](LICENSE-MIT) for details.
