# Welle

Welle is a tool for benchmarking servers similar to [ApacheBench](https://httpd.apache.org/docs/2.4/programs/ab.html).

## Usage

```txt
USAGE:
    welle [OPTIONS] <URL> --num-requests <NUMBER>

FLAGS:
    -h, --help       Prints help information
    -V, --version    Prints version information

OPTIONS:
    -c, --concurrent-requests <NUMBER>    Number of in flight requests allowed at a time [default: 1]
    -m, --method <METHOD>                 HTTP method to use [default: GET]
    -n, --num-requests <NUMBER>           Total number of requests to make

ARGS:
    <URL>    URL to request
```

## Building

The tool requires `Rust` and `Cargo` which you can get [here](https://rustup.rs/). Once Rust and Cargo are installed, building is as easy as:

```bash
cargo build --release
```

And you can find your binary in "./target/release/welle".

## Roadmap

* [ ] Customization the type of request made
* [ ] Ability to log structured result data
* [ ] Graphing and charting of data
* [ ] Finer tuned diagnostics of how long individual parts of the request take (e.g., connection time)
* [ ] Control of how the test runs over time
