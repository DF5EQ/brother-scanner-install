install Brother scanner in Linux Mint 20 with brscan2-0.2.5-1.amd64

the following files are installed by brscan2-0.2.5-1.amd64.deb as shown:
this information was extracted from the deb package

  libsane-brother2.so         to  /usr/lib64/sane/    as link to libsane-brother2.so.1.0.7
  libsane-brother2.so.1       to  /usr/lib64/sane/    as link to libsane-brother2.so.1.0.7
  libsane-brother2.so.1.0.7   to  /usr/lib64/sane/    as library
  libbrcolm2.so               to  /usr/lib64/         as link to libbrcolm2.so.1.0.1
  libbrcolm2.so.1             to  /usr/lib64/         as link to libbrcolm2.so.1.0.1
  libbrcolm2.so.1.0.1         to  /usr/lib64/         as library
  libbrscandec2.so            to  /usr/lib64/         as link to libbrscandec2.so.1.0.0
  libbrscandec2.so.1          to  /usr/lib64/         as link to libbrscandec2.so.1.0.0
  libbrscandec2.so.1.0.0      to  /usr/lib64/         as library

the following files are searched by sane* in the shown directories
this information was retrieved with:
    sudo strace -f scanimage
    SANE_DEBUG_DLL=5 scanimage -L

libsane-brother2.so.1   /usr/lib/x86_64-linux-gnu/sane/
                        /usr/lib/sane/
                        /usr/lib64/sane/

libbrcolm2.so           /lib/x86_64-linux-gnu/tls/x86_64/x86_64/
                        /lib/x86_64-linux-gnu/tls/x86_64/
                        /lib/x86_64-linux-gnu/tls/
                        /lib/x86_64-linux-gnu/x86_64/x86_64/
                        /lib/x86_64-linux-gnu/x86_64/
                        /lib/x86_64-linux-gnu/
                        /usr/lib/x86_64-linux-gnu/tls/x86_64/x86_64/
                        /usr/lib/x86_64-linux-gnu/tls/x86_64/
                        /usr/lib/x86_64-linux-gnu/tls/
                        /usr/lib/x86_64-linux-gnu/x86_64/x86_64/
                        /usr/lib/x86_64-linux-gnu/x86_64/
                        /usr/lib/x86_64-linux-gnu/
                        /lib/tls/x86_64/x86_64/
                        /lib/tls/x86_64/
                        /lib/tls/
                        /lib/x86_64/x86_64/
                        /lib/x86_64/
                        /lib/
                        /usr/lib/tls/x86_64/x86_64/
                        /usr/lib/tls/x86_64/
                        /usr/lib/tls/
                        /usr/lib/x86_64/x86_64/
                        /usr/lib/x86_64/
                        /usr/lib/

libbrscandec2.so        /lib/x86_64-linux-gnu/
                        /usr/lib/x86_64-linux-gnu/
                        /lib/
                        /usr/lib/

the following actions are to do:

  libsane-brother2.so         nothing to do, not used
  libsane-brother2.so.1       can stay in /usr/lib64/sane/
  libsane-brother2.so.1.0.7   nothing to do, not used
  libbrcolm2.so               copy to a searched directory
  libbrcolm2.so.1             nothing to do, not used
  libbrcolm2.so.1.0.1         nothing to do, not used
  libbrscandec2.so            copy to a searched directory
  libbrscandec2.so.1          nothing to do, not used
  libbrscandec2.so.1.0.0      nothing to do, not used

but for consistency all will be symlinked to /usr/lib/x86_64-linux-gnu
