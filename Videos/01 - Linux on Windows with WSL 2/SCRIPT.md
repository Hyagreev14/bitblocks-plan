# Video 01 — Narration Script

**Working title:** Linux on Windows? What Is WSL 2 and Why Use It?  
**Format:** Explainer + practical demonstration  
**Target duration:** 7–10 minutes  
**Status:** Draft. Adapt after recording; do not read stage directions aloud.

The spoken wording is intentionally conversational. The creator can change phrases to sound natural. Anything in square brackets is a visual or production cue, not narration.

---

## 0:00 — Hook

[VISUAL: Start on a clean Windows desktop. Open the Ubuntu terminal. Cut between a Windows app and the Linux terminal. Show a few terminal commands quickly.]

**VOICEOVER:**

What if you could use Linux tools on your Windows PC without replacing Windows, setting up a separate traditional virtual machine, or constantly switching between operating systems?

That's exactly the problem Windows Subsystem for Linux is designed to solve.

In this video, I'll explain what WSL 2 actually is, why developers use it, and show you what running Linux inside Windows looks like on my own machine.

[ON SCREEN TEXT: LINUX + WINDOWS, ON ONE PC]

## 0:25 — The problem

[VISUAL: Show Windows desktop, then a terminal. Use a simple graphic: Windows apps on one side, Linux tools on the other.]

**VOICEOVER:**

Windows is a perfectly capable place to develop software. But a lot of developer tools, tutorials, scripts, and server workflows are designed around Linux.

You might want to use Bash, Linux command-line utilities, or a development environment that behaves more like a Linux server.

One option is to install Linux separately. Another is to use a virtual machine. Both can be useful, but they may be more setup than you need if your goal is simply to use Linux tools alongside your normal Windows apps.

That's where WSL comes in.

## 1:15 — What is WSL?

[VISUAL: Show the official name on screen: Windows Subsystem for Linux. Then a simple diagram: Windows → WSL → Linux distribution such as Ubuntu.]

**VOICEOVER:**

WSL stands for Windows Subsystem for Linux. It's a Windows feature that lets you install and run a Linux environment directly on your Windows computer.

You can install a Linux distribution such as Ubuntu or Debian, open its terminal, and use Linux command-line tools while still using Windows applications.

So instead of choosing Windows or Linux every time you want to work, you can use both on the same computer.

But there's one important detail: WSL has two versions, WSL 1 and WSL 2. They work differently under the hood.

This video focuses on WSL 2, which is the version I'm using.

## 2:30 — How WSL 2 works

[VISUAL: Simple animated diagram. Windows host at the bottom; a lightweight managed VM layer; Linux kernel and Ubuntu environment above it. Keep labels short.]

**VOICEOVER:**

WSL 2 uses virtualization technology to run a real Linux kernel inside a lightweight virtual machine managed by Windows.

That means it isn't simply pretending to be Linux, and it isn't just a collection of Linux-looking commands. It provides a Linux kernel for the environment.

The useful part is that Windows manages the virtual machine for you. You don't have to set up and operate a traditional virtual machine in the same way you normally would.

Your Linux distribution runs in that WSL environment, and Windows and Linux can work together. You can use Windows apps and Linux command-line tools on the same PC.

There are still differences between WSL and a full Linux installation, and WSL isn't the right tool for every situation. But for many development workflows, that integration is the main attraction.

## 3:30 — A look at my WSL setup

[VISUAL: Open a clean PowerShell window. Run the commands one at a time. Blur or crop account names and unrelated paths.]

**VOICEOVER:**

Let's take a look at what this actually looks like.

First, from PowerShell, I can ask WSL for its status.

[ON SCREEN COMMAND: `wsl --status`]

This gives me information about the WSL setup on this computer.

I can also list the Linux distributions installed on the machine and see which WSL version each one is using.

[ON SCREEN COMMAND: `wsl --list --verbose`]

Here, my Ubuntu distribution is running on WSL 2.

[VISUAL: Open Ubuntu terminal.]

And this is the Ubuntu terminal. It looks like a Linux shell because that's what it is: a Linux environment running through WSL.

I can check the kernel information with:

[ON SCREEN COMMAND: `uname -r`]

And I can check where I am in the Linux filesystem with:

[ON SCREEN COMMAND: `pwd`]

The important thing to notice is that I'm not in a separate Linux computer that I have to switch over to. I'm using a Linux environment from my Windows desktop.

## 5:00 — A tiny practical example

[VISUAL: Type commands slowly. Show the output clearly.]

**VOICEOVER:**

Let's do one small example.

I'll create a folder in my Linux home directory for this demonstration.

[ON SCREEN COMMANDS:]

```bash
mkdir -p ~/bitblock-wsl-demo
cd ~/bitblock-wsl-demo
```

Now I'll create a simple text file:

```bash
printf 'Hello from Linux on Windows!\n' > hello.txt
```

And read it back:

```bash
cat hello.txt
```

That's a tiny example, but it shows the basic idea. I'm using ordinary Linux commands, working inside the Linux filesystem, while Windows is still my main desktop.

I can even open the current folder in Windows File Explorer:

[ON SCREEN COMMAND: `explorer.exe .`]

[VISUAL: Show File Explorer opening the demo folder. Hide the personal Windows account name in the path.]

This Windows-and-Linux integration is one of the things that makes WSL useful.

## 6:15 — Why would you use it?

[VISUAL: Show quick labelled examples: Bash terminal, code editor, project folder, Docker icon only if actually installed and shown.]

**VOICEOVER:**

So why would someone use WSL?

If you're learning Linux, it gives you a way to practise Linux commands without replacing your Windows installation.

If you're developing software, it can give you a Linux environment for tools and workflows that expect Linux.

And if you're following a tutorial that uses Bash or Linux commands, WSL can make it easier to follow along from a Windows PC.

It's also useful when you want to keep your usual Windows apps while using Linux tools in the same workflow.

## 7:00 — Limitations and things to know

[VISUAL: Return to a clean terminal and show a short list of balanced points.]

**VOICEOVER:**

But WSL isn't magic, and it isn't a perfect replacement for every Linux setup.

WSL 2 uses virtualization, so it still depends on your computer's resources.

There can also be differences in performance depending on where your project files are stored and which tools you're using. For many Linux-heavy workflows, keeping project files in the Linux filesystem is a good starting point.

And if you need to learn how a traditional Linux server behaves, manage a full desktop Linux installation, or work with hardware in a very specific way, a separate Linux machine or virtual machine may still make more sense.

The point isn't that WSL is always better. It's that WSL is a convenient option for using Linux alongside Windows.

## 8:00 — Closing

[VISUAL: Show the terminal beside the Windows desktop. End on the BitBlock logo and tagline.]

**VOICEOVER:**

So that's WSL 2: a Windows-managed way to run a real Linux environment alongside Windows.

If you've been curious about Linux but don't want to leave Windows behind, it's definitely worth understanding.

This is the first video on BitBlock, where we'll explore software, technology, experiments, and the process of building things.

If that sounds interesting, subscribe and come explore with me.

CODE. CREATE. EXPLORE.

---

## Recording adaptation notes

- The script is a guide, not a word-for-word performance requirement.
- Verify that every command works on the actual recording machine before recording the final take.
- If `explorer.exe .` does not open the intended folder, omit that moment rather than pretending it worked.
- Replace any generic description with what the screen actually shows.
- Do not read version numbers unless they are visible and verified at recording time.
- If the final video is shorter or longer, update chapter timestamps after the edit.
- Keep the tone curious and explanatory. Avoid presenting WSL as the only correct way to use Linux.
