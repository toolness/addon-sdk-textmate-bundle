This is a simple TextMate bundle for Mozilla's Add-on SDK.

## Setup

Go to **TextMate > Preferences... > Advanced > Shell Variables** and add a new environment variable called `ADDON_SDK_ROOT`. Set it to the absolute path of your Add-on SDK installation root.

## Usage

Before running or testing your add-on, you should use the **Start Firefox in Development Mode** command. This will open a new Terminal window and run `cfx develop` in it, which opens Firefox and sets up a little server that waits for jobs to be sent to it. Any logging messages will also be displayed in this Terminal window, so you'll want to keep it visible at all times.

Now open any file of your add-on package in TextMate.

Use the **Run Add-on in Firefox** command to issue a job that loads the add-on in Firefox. This is analogous to `cfx run`.

Use the **Test Add-on in Firefox** command to run your add-on's test suite. This is analogous to `cfx test`.

## Limitations

Currently, [bug 615060][] causes a noticeable delay between issuing a run/test command in TextMate and seeing its effect.

You'll probably want to also open Firefox's Error Console to see any messages that don't make their way to the Terminal window.

  [bug 615060]: https://bugzilla.mozilla.org/show_bug.cgi?id=615060
