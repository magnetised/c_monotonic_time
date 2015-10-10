# C Monotonic Time

An Erlang module to retrieve a monotonic time value directly from the OS using
a NIF.

I *know* that Erlang/OTP 18 has fantasic time functions but I needed something
that was more consistent with time functions available in C in order to
coordinate with an audio port driver.

## Usage

    $ rebar compile
    $ erl -pa ebin
    1> c_monotonic_time:microseconds().
    7311345180
    2> c_monotonic_time:milliseconds().
    7316529

