Go Clui
=======

Opiniated, minimalistic and multi platform UI library for Golang command line apps.


Import the library:

```Go
    import (
        "github.com/enr/clui"
    )
```

Using Clui, an UI has:

- Layout: the output style, eg plain or machine readable
- VerbosityLevel: how to filter output
- Interactive: if wait for user's answers

Creation of a default `Clui`:

```Go
    ui, err := clui.NewClui()
```

Creation with configuration:

```Go
    verbosity := func(ui *clui.Clui) {
        ui.VerbosityLevel = clui.VerbosityLevelHigh
    }
    ui, _ := clui.NewClui(verbosity)
```

See `examples` directory for more.

License
-------

A lot of code of this library was taken from Packer UI released under the same license (Mozilla Public License Version 2.0).

Mozilla Public License Version 2.0 - see LICENSE file.

Copyright 2015 clui contributors

