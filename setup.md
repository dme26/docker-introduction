---
title: Setup
---
### Website accounts to create
Please seek help at the start of the lesson if you have not been able to establish website accounts on both of:
- The [Docker Hub](http://hub.docker.com). We will use the Docker Hub to download pre-built container images, and for you to upload and download container images that you create, as explained in the relevant lesson episodes.
- [Bitbucket](http://bitbucket.org) is a code project repository site, akin to [GitHub](https://github.org). We will use Bitbucket to create a Docker container from a Docker image that you create.

### Software to install
Unfortunately, in many common situations installing Docker on your laptop will not straightforward if you do not have a large amount of technical experience. We try to have workshop helpers on-hand who have worked their way through the install process.

Even if you are unsuccessful in installing Docker on your laptop, you can still complete some parts of this Docker lesson, just using a web browser. At worst you will still see the instructor demonstrate use of the Docker tools.

Please try to install the appropriate software from the list below depending on the operating system that your laptop is running:
- Microsoft Windows, either:
    - Try this first, although it won't work with Windows 10 Home Edition. Install the [Docker Desktop (Windows)](https://hub.docker.com/editions/community/docker-ce-desktop-windows), or failing that;
    - Install the [Docker Toolbox (Windows)](https://docs.docker.com/toolbox/toolbox_install_windows/).
- Apple macOS, either:
    - Try this first, although it will not work with older versions of macOS. Install the [Docker Desktop (Mac)](https://hub.docker.com/editions/community/docker-ce-desktop-mac), or failing that:
    - Install the [Docker Toolbox (Mac)](https://docs.docker.com/toolbox/toolbox_install_mac/).
- Linux: there are too many varieties of Linux to give precise instructions here, but hopefully you can locate documentation for getting Docker installed on your Linux distribution. It may already be installed. Note that Docker do list a number of versions of the Docker Engine for different Linux distributions, at <https://hub.docker.com/search/?type=edition&offering=community>

### A quick tutorial on copy/pasting file contents from episodes of the lesson
Let's say you want to copy text off the lesson website and paste it into a file named `myfile` in the current working directory of a shell window. This can be achieved in many ways, depending on your laptop's operating system, but routes I have found work for me:
- macOS and Linux: you are likely to have the `nano` editor installed, which provides you with a very straightforward way to create such a file, just run `nano myfile`, then paste text into the shell window, and press <kbd>control</kbd>+<kbd>x</kbd> to exit: you will be prompted whether you want to save changes to the file, and you can type <kbd>y</kbd> to say "yes".
- Microsoft Windows running `cmd.exe` shells: 
  - `del myfile` to remove `myfile` if it already existed;
  - `copy con myfile` to mean what's typed in your shell window is copied into `myfile`;
  - paste the text you want within `myfile` into the shell window;
  - type <kbd>control</kbd>+<kbd>z</kbd> and then press <kbd>enter</kbd> to finish copying content into `myfile` and return to your shell;
  - you can run the command `type myfile` to check the content of that file, as a double-check.
- Microsoft Windows running PowerShell:
  - The `cmd.exe` method probably works, but another is to paste your file contents into a so-called "here-string" between `@'` and `'@` as in this example that follows (the ">" is the prompt indicator):

        > @'
        Some hypothetical
        file content that is
        
        split over many
        
        lines.
        '@ | Set-Content myfile -encoding ascii

{% include links.md %}

{% comment %}
<!--  LocalWords:  myfile kbd links.md md endcomment
-->
{% endcomment %}
