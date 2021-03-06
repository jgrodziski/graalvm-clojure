# Clojure meets GraalVM

This project contains a set of "hello world" projects to verify which
Clojure libraries do actually compile and produce **native images**
under GraalVM.

Here the instructions on how to build your own Clojure projects with GraalVM.

  - [Build a "Hello world!" project](./doc/clojure-graalvm-native-binary.md)


Here the list of libraries tested:

  - [Clojure core](./clojure) :white_check_mark:
  - [amazonica/s3](./amazonica-s3) :x: (*Buildtime and Runtime error*)
  - [cheshire](./cheshire) :white_check_mark:
  - [nippy](./nippy) :warning: (*Can't serialize exceptions*)
  - cognitect/aws-api+s3 :question:
  - ring/jetty :question:
  - ring/http-kit :question:
  - ring/aleph :question:
  - safely :question:


More libraries to come (*PRs are welcome*).


## License

Copyright © 2019 Bruno Bonacci

Distributed under the Apache License v 2.0 (http://www.apache.org/licenses/LICENSE-2.0)
