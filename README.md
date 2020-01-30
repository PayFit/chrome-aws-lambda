# @payfit/chrome-aws-lamnda

This project was forked from `chrome-aws-lambda` in order to change the `bin/chromium.br` file.
Latest version of chrome-aws-lambda (2.0.0) was shipping chromium v79 at the time of writing, and rendering of our payslip was messed up by any version of chrome above v66.

So this repo allows us to inject the latest possible version we can support of chromium in our `apps`'s lambda in order to enable us to move to node 12 before node 8's end of life in february 2020.

_NB: new commits pushed on `master` will automagically trigger a circle ci pipeline which will try to publish the package to NPM. It'll fail if you have not changed the version in `package.json`._

