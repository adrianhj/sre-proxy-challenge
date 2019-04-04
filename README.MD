# SRE Proxy Challenge

To understand where your thinking is at when it comes to deploying, maintaining, and operating infrastructure--we would like you to deploy a secure reverse proxy or web server using the toolchain and stack of your choice.

It's important to note that it's by no means a test with a single correct answer, we just want to get a sense for how you approach infrastructure, code in production, and solving problems.

The reverse proxy or web server should:

* Listen on port 80 and 443
* Re-direct any non-HTTPS requests to HTTPS
* Provide HTTPS over 443 using a certificate signed by a local CA set-up
* Respond with a `text/plain` content of "Hello SRE!" from a source of your choice of:
    * Statically served, or
    * Proxying onto a small backing service provided by yourself

Please also add a supporting automated test using your language/framework of choice asserting that:

* Requests are succesfully served via HTTPS on port 443
* The content "Hello SRE!" is returned using `text/plain`

As observability is the foundation for us to build the future we envision, please also support it with a small monitoring set-up tracking a few basic SLIs; again using stack of your choice that is suitable for this challenge.

## Things that interest us:

* Infrastructure as code and containerisation, especially using declarative paradigms
* Bullet-proof production allowing our product engineers to make high-impact changes on a continous basis with confidence
* Sublinear scaling of our operational workload as we grow our customer base

## Submitting your challenge:

* The challenge must be shared as a git repository
* You can either create a public repository on your favourite git hosting provider (GitHub, GitLab, BitBucket) and share the link
* Or send the whole repository, zipped (including the .git directory!)
* Please include both build and run instructions, we use a mix of Windows and Mac on our end

Important, please only submit your challenge when you feel you are completely done!