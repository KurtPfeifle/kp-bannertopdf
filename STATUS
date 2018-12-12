

Code is working on the command line, but not yet been thoroughly tested.

Testing happened on the command line with this command:

     ./kp-bannertopdf           \
            888888              \
            kp                  \
            "KP-Banner-Test"    \
            13                  \
            "media=yellow sides=two-sided finishings=3 markdown=false job-originating-host-name=MacBook" \
            reference-banner

There are some 'xdg-open' commands to serve for debugging.
These will go away when in production.

Currently, the filter uses HTML as its intermediate format.
From HTML it creates TWO output PDF files:

* one with the help of a 'pandoc' command,
* the other with the help of a 'htmldoc' command.

Both are saved to a temporary file.
For real usage as a banner-to-pdf filter, output needs to go to stdout.

I used Pandoc v2.1.3 and HTMLdoc v1.9.5 for my tests.
Should test with older versions and then recommend a minimum version.

