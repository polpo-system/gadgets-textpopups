# gadgets-textpopups

TextPopups for the gadgets of [polpo](https://github.com/polpo-system/polpo), on x86: popup menus in
text documents, shown with a click outside the text: commands for the kind of file (by its suffix),
the recent files, and the procedures and types declared in the text, to jump to.

```
portia.Install gadgets-textpopups
```

## Using

    TextPopups.Install    popup menus on
    TextPopups.Remove     popup menus off

The menus are described in TextPopups.Text; `tools/TextPopups.Tool` (from Linux Oberon) explains
the description.

## What is here

    src/TextPopups.Mod       the popup menus
    share/TextPopups.Text    the menus
    tools/TextPopups.Tool
    test/TextPopupsTest.Mod

It uses the modules of the x86 compiler (OPS, OPM, OPT), so the package installs on x86 only. The source comes from ETH Linux Oberon (OLR, 2017-06-18), converted from an Oberon text to
plain text; the first commit has it unchanged.

## Tests

    TextPopupsTest.Run      1 check: the module loaded; it needs the desktop's display (on x86)

The license is GPL-3 (`LICENSE`); the code comes from ETH Oberon, whose license (`LICENSE.ETH`)
asks to keep its copyright notice and conditions, which `LICENSE.ETH` does.
