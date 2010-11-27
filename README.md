This is a simple TextMate bundle for Mozilla's Add-on SDK.

## Setup

Go to **TextMate > Preferences... > Advanced > Shell Variables** and add a new environment variable called `ADDON_SDK_ROOT`. Set it to the absolute path of your Add-on SDK installation root.

## Usage

Before you use any other commands in the bundle, you should use the **Start Firefox in Development Mode** command. This will open a new Terminal window and run `cfx develop` in it, which opens Firefox and sets up a little server that waits for jobs to be sent to it. Any console messages from the jobs will be displayed in this Terminal window.

Now open any file of your add-on package in TextMate.

Use the **Run Add-on in Firefox** command to issue a job that loads the add-on in Firefox. This is analogous to `cfx run`.

Use the **Test Add-on in Firefox** command to run your add-on's test suite. This is analogous to `cfx test`.
