-   31/10/2018: v0.1.0

    *   Initial release of WebPShop, a Photoshop plug-in for reading and writing
        WebP files.
    *   Handles animations too.

-   01/03/2019: v0.1.1

    *   Updated to Adobe Photoshop Plug-In and Connection SDK CC 2019
        (posix i/o for Mac, no handle lock).
    *   Updated to WebP 1.0.2.
    *   Tested on Windows Server 2016 Datacenter with Photoshop CC 2018
        (v 19.1.7) x64, CC 2019 (v.20.0.3) x64, Release and Debug.

-   15/03/2019: v0.2.0

    *   Now compiles with XCode.
    *   Added Cocoa interface implementation for Mac (encoding settings window
        and About box).
    *   Tested on a MacBook Pro (macOS Mojave 10.14.3) with Photoshop CC 2019
        (v 20.0.3 and 20.0.4).

-   24/04/2019: v0.2.1

    *   Adapted UI quality and compression mappings to WebP encoding settings.
    *   Tested on Windows Server 2016 Datacenter with Photoshop CC 2019
        (v 20.0.4) x64, Release.

-   29/04/2020: v0.3.0

    *   Added the "Loop forever" checkbox for animations.
    *   Added metadata import/export from/to WebP through the "Keep EXIF",
        "Keep XMP" and "Keep Color Profile" checkboxes.
    *   Tested on Windows Server 2016 Datacenter with Photoshop 2020
        (v 21.1.2) x64, Release.

-   26/06/2020: v0.3.1

    *   Fix inaccuracies in WebPShop.r resource file.
    *   Fix PIUtilities.r MacOS ResMerger warning.
    *   Add directions in README.md.

-   05/02/2021: v0.3.2

    *   Updated to Adobe Photoshop Plug-In and Connection SDK 2021 v2.
    *   Updated to WebP 1.2.0.
    *   Built with Microsoft Visual Studio Community 2017 15.8.3 and
        Apple XCode 12.4 (12D4e).
    *   Tested on Windows Server 2016 Datacenter with Photoshop 2021
        (v 22.1.1) x64, Release.
    *   Tested on macOS Catalina Version 10.15.7 with Photoshop 2020
        (v 21.2.4) and Photoshop 2021 (v 22.1.1) x64, Release.

-   09/04/2021: v0.3.3

    *   Built with Microsoft Visual Studio Community 2019 16.9.2.
    *   Removed the Windows x86 architecture target.
    *   Added the Windows ARM64 architecture target.
    *   Tested on Windows Server 2016 Datacenter with Photoshop 2021
        (v 22.3.0) x64, Release.

-   29/06/2021: v0.3.4

    *   Fixed the opening of animated WebP images as Smart Objects.

-   14/09/2021: v0.4.0

    *   Updated to WebP 1.2.1.
    *   Added 16 and 32 bits/channel support.
    *   Display an error prompt instead of hiding WebP export when
        saving an image of another Mode than RGB Color.
    *   Built with Microsoft Visual Studio Community 2019 16.11.0.
    *   Tested on Windows Server 2016 Datacenter with Photoshop 2021
        (v 22.5.1) x64, Release.
