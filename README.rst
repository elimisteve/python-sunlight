python-sunlight
===============

This project is an attempt to unify all the Sunlight API bindings into a single
project that is clear, concise, easy to read, powerful, and fun to play with.

Setup
*****

Using this library is very easy - by default, python-sunlight will search for
API keys in two places. First, ``~/.sunlight.key`` will be read, and the
contents of that file will be used as the API Key. Secondly, if an enviroment
variable called ``SUNLIGHT_API_KEY`` is set, that will be used (in the case of
both being read, the enviroment variable *will* override the file.)

To register for an API key, if you don't have one, please fill out the form
`here <http://services.sunlightlabs.com/accounts/register/>`_.

The easiest way to write this file out is by running a command similar to this
( on systems that support a POSIX shell):

    echo "API_KEY" > ~/.sunlight.key

where `API_KEY` is actually the string of letters and numbers that was emailed
to you. Actually putting `API_KEY` into this file will most likely result in 
an error from the server. You can confirm they key with the following command:

    cat ~/.sunlight.key

This should output the string that was emailed to you.

Help me!
********

Basic usage and some brief examples can be found on
`readthedocs <http://python-sunlight.rtfd.org>`_.
If this doens't help, feel free to email for help, ask over IRC in
``#sunlightlabs`` on ``irc.freenode.net``, or open a issue if it's a
particularly nasty bug (particularly regarding ambiguous documentation, or
poorly exposed API methods). 

License
*******

All code in this project is licensed under a BSD-3 clause style license. The
exact terms are in the `LICENSE` file, which will be distributed with any
copy of the source you recieve.

Contribute
**********

Bugfixes, documentation contributions and more extensive (yet clear) example
scripts are all welcome and encouraged. Please open a pull-request against
python-sunlight, or email a format-patch to the email address listed in the
setup.py script.
