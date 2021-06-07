# JSSOFTWARE_Android_rejuvenation
This public repository includes raw data used in the experimental analysis provided in the article "*Software Micro-Rejuvenation for Android Mobile Systems*".

The repository contains four folders referring to the four experiments provided in the article. Each folder contains two kind of files: 

1. The ***displayed.txt*** file, which contains rows identifying the Android activity for target applications with the related *Launch Time* at specific timestamp during the experiment;

2. The ***meminfo.txt*** file, which contains the snapshot of how application's memory is divided between different types of RAM allocation during the experiment; we leverage the output of the **dumpsys** tool (https://developer.android.com/studio/command-line/dumpsys) specifying the ``meminfo`` option;

Each folders is related to the following experiments:

* **REJ_NO_REJUVENATION** the scenario without performing rejuvenation on the device;

* **REJ_AM** the scenario in which rejuvenation is performed only against ``ActivityManager`` service;

* **REJ_AM_WIFI** the scenario in which rejuvenation is performed against both ``ActivityManager`` and ``WiFiService`` service;

* **REJ_AM_WIFI_PM** the scenario in which rejuvenation is performed against ``ActivityManager``, ``WiFiService``, and ``PowerManager `` service;

