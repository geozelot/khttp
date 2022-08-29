### Collect & Merge Fork!
#### This repository is meant to collect some of the most recent works across forks.

#### Any help with maintenance and further development appreciated.
#
____
# khttp
[![License](https://img.shields.io/github/license/jkcclemens/khttp.svg)](https://github.com/jkcclemens/khttp/blob/master/LICENSE)

khttp is a simple library for HTTP requests in Kotlin. It functions similarly to Python's `requests` module.

```kotlin
import khttp.get

fun main(args: Array<out String>) {
    // Get our IP
    println(get("http://httpbin.org/ip").jsonObject.getString("origin"))
    // Get our IP in a simpler way
    println(get("http://icanhazip.com").text)
}
```