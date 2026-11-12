# Video 01 — Narration Script

**Working title:** How to Install Linux on Windows with WSL 2 (Beginner Guide)  
**Format:** Explainer + guided installation walkthrough + practical demonstration  
**Target duration:** 9–11 minutes  
**Status:** Draft. Adapt after recording; do not read stage directions aloud.

The spoken wording is intentionally conversational. The creator can change phrases to sound natural. Anything in square brackets is a visual or production cue, not narration.

---

## 0:00 — Hook

[VISUAL: Start on a clean Windows desktop. Open the Ubuntu terminal. Cut between a Windows app and the Linux terminal. Show a few terminal commands quickly. Then flash the words “INSTALL WSL 2”.]

**VOICEOVER:**

What if you could add a Linux environment to your Windows PC without replacing Windows?

That's what Windows Subsystem for Linux, or WSL, lets you do.

In this video, I'll explain what WSL 2 actually is, walk you through the standard way to install it with Ubuntu on a supported Windows PC, and then show you a real Linux terminal and a few commands on my own setup.

[ON SCREEN TEXT: LINUX ON WINDOWS — WSL 2]

## 0:25 — The problem

[VISUAL: Show Windows desktop, then a terminal. Use a simple graphic: Windows apps on one side, Linux tools on the other.]

**VOICEOVER:**

Windows is a perfectly capable place to develop software. But a lot of developer tools, tutorials, scripts, and server workflows are designed around Linux.

You might want to use Bash, Linux command-line utilities, or a development environment that behaves more like a Linux server.

One option is to install Linux separately. Another is to use a virtual machine. Both can be useful, but they may be more setup than you need if your goal is simply to use Linux tools alongside your normal Windows apps.

That's where WSL comes in.

## 1:05 — What is WSL?

[VISUAL: Show the official name on screen: Windows Subsystem for Linux. Then a simple diagram: Windows → WSL → Linux distribution such as Ubuntu.]

**VOICEOVER:**

WSL stands for Windows Subsystem for Linux. It's a Windows feature that lets you install and run a Linux environment directly on your Windows computer.

You can install a Linux distribution such as Ubuntu or Debian, open its terminal, and use Linux command-line tools while still using Windows applications.

So instead of choosing Windows or Linux every time you want to work, you can use both on the same computer.

But there's one important detail: WSL has two versions, WSL 1 and WSL 2. They work differently under the hood.

This video focuses on WSL 2, which is the version I'm using.

## 2:10 — How WSL 2 works

[VISUAL: Simple animated diagram. Windows host at the bottom; a lightweight managed VM layer; Linux kernel and Ubuntu environment above it. Keep labels short.]

**VOICEOVER:**

WSL 2 uses virtualization technology to run a real Linux kernel inside a lightweight virtual machine managed by Windows.

That means it isn't simply pretending to be Linux, and it isn't just a collection of Linux-looking commands. It provides a Linux kernel for the environment.

The useful part is that Windows manages the virtual machine for you. You don't have to set up and operate a traditional virtual machine in the same way you normally would.

Your Linux distribution runs in that WSL environment, and Windows and Linux can work together. You can use Windows apps and Linux command-line tools on the same PC.

There are still differences between WSL and a full Linux installation, and WSL isn't the right tool for every situation. But for many development workflows, that integration is the main attraction.

## 3:00 — Before you install

[VISUAL: Simple compatibility card: “Windows 11” or “Windows 10 — version 2004 / build 19041 or later”. Show a small “Check with winver” label.]

**VOICEOVER:**

Before installing, check that your Windows version supports the simple installation command.

Microsoft documents this one-command method for Windows 11 and Windows 10 version 2004, build 19041, or later.

If you're on an older Windows version, the process can be different, so use Microsoft's manual installation guide linked in the description rather than blindly following this exact path.

## 3:30 — Installing WSL 2 and Ubuntu

[VISUAL: Clearly label this as “FRESH WINDOWS SETUP”. Show a clean PowerShell window graphic with the command typed. Do not present it as a live install on the creator's already-configured PC.]

**VOICEOVER:**

On a fresh supported Windows PC, open PowerShell as Administrator.

Then enter this command:

[ON SCREEN COMMAND:]

~~~powershell
wsl --install
~~~

By default, this installs Ubuntu.

The command enables the Windows components WSL needs, downloads and installs the Linux kernel, sets WSL 2 as the default for new installations, and installs Ubuntu.

Restart your computer if Windows asks you to.

[VISUAL: Step graphic: 1. PowerShell as Administrator → 2. wsl --install → 3. Restart.]

One note: WSL is already installed on my computer, so I'm not going to uninstall or reinstall my working setup just to capture this. These are the standard fresh-install steps, and I'll show you the real WSL setup on my machine in a moment.

## 4:45 — First launch and verification

[VISUAL: Show a simple Ubuntu first-launch illustration or clean screen capture if available. Do not show or record any real password entry.]

**VOICEOVER:**

After restarting, open Ubuntu from the Start menu.

The first launch may take a little while because Windows needs to finish setting up the distribution.

You'll then be asked to create a Linux username and password. These are for your Ubuntu environment; they are separate from your Windows account.

One thing that surprises new users: when you type the password, nothing appears on screen. No dots, no stars, nothing. That's normal. Type it and press Enter.

Once setup is complete, open PowerShell and run:

[ON SCREEN COMMAND:]

~~~powershell
wsl --list --verbose
~~~

This lists your installed Linux distributions and shows which WSL version each one is using. For this video, the important thing is that the Ubuntu entry shows version 2.

You can also run:

~~~powershell
wsl --status
~~~

to see the overall WSL status.

If you want a different Linux distribution, you can list the available ones with **wsl --list --online** and install one by name. But Ubuntu is a straightforward starting point for this walkthrough.

## 5:45 — A look at my WSL setup

[VISUAL: Show the creator's actual PowerShell output. Run the commands one at a time. Blur or crop account names and unrelated paths.]

**VOICEOVER:**

Now let's look at an actual WSL setup.

First, here's the status on my computer.

[ON SCREEN COMMAND: wsl --status]

And here's the list of installed distributions.

[ON SCREEN COMMAND: wsl --list --verbose]

Here, my Ubuntu distribution is running on WSL 2.

[VISUAL: Open Ubuntu terminal.]

And this is the Ubuntu terminal. It looks like a Linux shell because that's what it is: a Linux environment running through WSL.

I can check the kernel information with:

[ON SCREEN COMMAND: uname -r]

And I can check where I am in the Linux filesystem with:

[ON SCREEN COMMAND: pwd]

The important thing to notice is that I'm using a Linux environment from my Windows desktop. I don't have to switch away from Windows to use it.

## 6:45 — A tiny practical example

[VISUAL: Type commands slowly. Show the output clearly.]

**VOICEOVER:**

Let's do one small example.

I'll create a folder in my Linux home directory for this demonstration.

[ON SCREEN COMMANDS:]

~~~bash
mkdir -p ~/bitblock-wsl-demo
cd ~/bitblock-wsl-demo
~~~

Now I'll create a simple text file:

~~~bash
printf 'Hello from Linux on Windows!\n' > hello.txt
~~~

And read it back:

~~~bash
cat hello.txt
~~~

That's a tiny example, but it shows the basic idea. I'm using ordinary Linux commands, working inside the Linux filesystem, while Windows is still my main desktop.

I can even open the current folder in Windows File Explorer:

[ON SCREEN COMMAND: explorer.exe .]

[VISUAL: Show File Explorer opening the demo folder. Hide the personal Windows account name in the path.]

This Windows-and-Linux integration is one of the things that makes WSL useful.

## 7:45 — Why would you use it?

[VISUAL: Show quick labelled examples: Bash terminal, code editor, project folder. Only show apps that are actually installed and relevant.]

**VOICEOVER:**

So why would someone use WSL?

If you're learning Linux, it gives you a way to practise Linux commands without replacing your Windows installation.

If you're developing software, it can give you a Linux environment for tools and workflows that expect Linux.

And if you're following a tutorial that uses Bash or Linux commands, WSL can make it easier to follow along from a Windows PC.

It's also useful when you want to keep your usual Windows apps while using Linux tools in the same workflow.

## 8:30 — Limitations and things to know

[VISUAL: Return to a clean terminal and show a short list of balanced points.]

**VOICEOVER:**

But WSL isn't magic, and it isn't a perfect replacement for every Linux setup.

WSL 2 uses virtualization, so it still depends on your computer's resources.

There can also be differences in performance depending on where your project files are stored and which tools you're using. For many Linux-heavy workflows, keeping project files in the Linux filesystem is a good starting point.

And if you need to learn how a traditional Linux server behaves, manage a full desktop Linux installation, or work with hardware in a very specific way, a separate Linux machine or virtual machine may still make more sense.

The point isn't that WSL is always better. It's that WSL is a convenient option for using Linux alongside Windows.

## 9:20 — Closing

[VISUAL: Show the terminal beside the Windows desktop. End on the BitBlock logo and tagline.]

**VOICEOVER:**

So that's WSL 2: a Windows-managed way to run a real Linux environment alongside Windows.

You now know the standard installation path, how to complete Ubuntu's first launch, and how to check that your distribution is using WSL 2.

If you've been curious about Linux but don't want to leave Windows behind, it's definitely worth exploring.

This is the first video on BitBlock, where we'll explore software, technology, experiments, and the process of building things.

If that sounds interesting, subscribe and come explore with me.

CODE. CREATE. EXPLORE.

---

## Recording adaptation notes

- The script is a guide, not a word-for-word performance requirement.
- The installation segment is a walkthrough for a fresh supported Windows PC. The creator's own PC already has WSL installed; do not uninstall, reset, or reinstall it for footage.
- Use a clearly labelled command/step graphic for the fresh-install sequence. Do not fake installer output or imply that the command was run live on the creator's machine.
- Verify that every command used on the actual recording machine works before recording the final take.
- If **explorer.exe .** does not open the intended folder, omit that moment rather than pretending it worked.
- Replace any generic description with what the screen actually shows.
- Do not read version numbers unless they are visible and verified at recording time.
- If the final video is shorter or longer, update chapter timestamps after the edit.
- Keep the tone curious and explanatory. Avoid presenting WSL as the only correct way to use Linux.
