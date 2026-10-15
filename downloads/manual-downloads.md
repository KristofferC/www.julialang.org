@def title = "Manual Downloads"

~~~
<div class="container pt-sm-2">
  <div class="row">
    <div class="col-lg-4 col-md-3 language-features"><hr/></div>
    <div class="col-lg-4 col-md-6 language-features section-heading">
      <h2 class="lead secondary-heading">Current Stable Release</h2>
    </div>
    <div class="col-lg-4 col-md-3 language-features"><hr/></div>
  </div>
  <br>
~~~

\note{Use juliaup for typical installations}{See the [installation instructions](/downloads/) on using `juliaup` to install the official Julia binaries. Users who are unable to use `juliaup` or require a specific, atypical setup may manually download and install the binaries from this page. If these binaries do not work for you, please [file an issue in the Julia project](https://github.com/JuliaLang/julia/issues).}

~~~
<h3 id="current_stable_release"><a href="#current_stable_release">v{{stable_release}} ({{stable_release_date}})</a></h3>
~~~

[Release notes](https://github.com/JuliaLang/julia/blob/v{{stable_release}}/NEWS.md) | [GitHub tag](https://github.com/JuliaLang/julia/releases/tag/v{{stable_release}}) | [SHA256 checksums](https://julialang-s3.julialang.org/bin/checksums/julia-{{stable_release}}.sha256) | [MD5 checksums](https://julialang-s3.julialang.org/bin/checksums/julia-{{stable_release}}.md5)

@@row @@col-12
~~~
<table class="downloads table table-hover table-bordered">
  <tbody>
    <tr>
      <th> Platform</th>
      <th> 64-bit</th>
      <th> 32-bit</th>
    </tr>
    <tr>
      <td> Windows <a href="/downloads/platform/#windows">[help]</a></td>
      <td> <a href="https://julialang-s3.julialang.org/bin/winnt/x64/{{stable_release_short}}/julia-{{stable_release}}-win64.exe">installer</a>, <a href="https://julialang-s3.julialang.org/bin/winnt/x64/{{stable_release_short}}/julia-{{stable_release}}-win64.zip">portable</a> </td>
      <td> <a href="https://julialang-s3.julialang.org/bin/winnt/x86/{{stable_release_short}}/julia-{{stable_release}}-win32.exe">installer</a>,  <a href="https://julialang-s3.julialang.org/bin/winnt/x86/{{stable_release_short}}/julia-{{stable_release}}-win32.zip">portable</a> </td>
    </tr>
    <tr>
      <td> macOS (Apple Silicon) <a href="/downloads/platform/#macos">[help]</a></td>
      <td> <a href="https://julialang-s3.julialang.org/bin/mac/aarch64/{{stable_release_short}}/julia-{{stable_release}}-macaarch64.dmg">.dmg</a>, <a href="https://julialang-s3.julialang.org/bin/mac/aarch64/{{stable_release_short}}/julia-{{stable_release}}-macaarch64.tar.gz">.tar.gz</a> </td>
      <td> </td>
    </tr>
    <tr>
      <td> macOS (Intel x86) <a href="/downloads/platform/#macos">[help]</a></td>
      <td> <a href="https://julialang-s3.julialang.org/bin/mac/x64/{{stable_release_short}}/julia-{{stable_release}}-mac64.dmg">.dmg</a>, <a href="https://julialang-s3.julialang.org/bin/mac/x64/{{stable_release_short}}/julia-{{stable_release}}-mac64.tar.gz">.tar.gz</a> </td>
      <td> </td>
    </tr>
    <tr>
      <td> Generic Linux on x86 <a href="/downloads/platform/#linux_and_freebsd">[help]</a></td>
      <td>
        <a href="https://julialang-s3.julialang.org/bin/linux/x64/{{stable_release_short}}/julia-{{stable_release}}-linux-x86_64.tar.gz">glibc</a>
        (<a href="https://julialang-s3.julialang.org/bin/linux/x64/{{stable_release_short}}/julia-{{stable_release}}-linux-x86_64.tar.gz.asc">GPG</a>)<!--,
        <a href="https://julialang-s3.julialang.org/bin/musl/x64/{{stable_release_short}}/julia-{{stable_release}}-musl-x86_64.tar.gz">musl</a><sup>[<a href=#musl-fn>1</a>]</sup>
        (<a href="https://julialang-s3.julialang.org/bin/musl/x64/{{stable_release_short}}/julia-{{stable_release}}-musl-x86_64.tar.gz.asc">GPG</a>)-->
      </td>
      <td> <a href="https://julialang-s3.julialang.org/bin/linux/x86/{{stable_release_short}}/julia-{{stable_release}}-linux-i686.tar.gz">glibc</a>
        (<a href="https://julialang-s3.julialang.org/bin/linux/x86/{{stable_release_short}}/julia-{{stable_release}}-linux-i686.tar.gz.asc">GPG</a>)
      </td>
    </tr>
    <tr>
      <td> Generic Linux on ARM <a href="/downloads/platform/#linux_and_freebsd">[help]</a></td>
      <td> <a href="https://julialang-s3.julialang.org/bin/linux/aarch64/{{stable_release_short}}/julia-{{stable_release}}-linux-aarch64.tar.gz">.tar.gz</a>
        (<a href="https://julialang-s3.julialang.org/bin/linux/aarch64/{{stable_release_short}}/julia-{{stable_release}}-linux-aarch64.tar.gz.asc">GPG</a>)
      </td>
      <td> <!-- <a href="https://julialang-s3.julialang.org/bin/linux/armv7l/{{stable_release_short}}/julia-{{stable_release}}-linux-armv7l.tar.gz">ARMv7-a hard float</a>
                                       (<a href="https://julialang-s3.julialang.org/bin/linux/armv7l/{{stable_release_short}}/julia-{{stable_release}}-linux-armv7l.tar.gz.asc">GPG</a>) -->
      </td>
    </tr>
    <!--
    <tr>
      <td> Generic Linux on PowerPC <a href="/downloads/platform/#linux_and_freebsd">[help]</a></td>
      <td> <a href="https://julialang-s3.julialang.org/bin/linux/ppc64le/{{stable_release_short}}/julia-{{stable_release}}-linux-ppc64le.tar.gz">little endian</a>
        (<a href="https://julialang-s3.julialang.org/bin/linux/ppc64le/{{stable_release_short}}/julia-{{stable_release}}-linux-ppc64le.tar.gz.asc">GPG</a>)
      </td>
      <td>
      </td>
    </tr>
    -->
    <tr>
      <td> Generic FreeBSD on x86 <a href="/downloads/platform/#linux_and_freebsd">[help]</a></td>
      <td> <a href="https://julialang-s3.julialang.org/bin/freebsd/x64/{{stable_release_short}}/julia-{{stable_release}}-freebsd-x86_64.tar.gz">.tar.gz</a>
        (<a href="https://julialang-s3.julialang.org/bin/freebsd/x64/{{stable_release_short}}/julia-{{stable_release}}-freebsd-x86_64.tar.gz.asc">GPG</a>)
      </td>
      <td> </td>
    </tr>
  </tbody>
</table>
<table>
  <tbody>
    <tr>
      <th> Source </th>
      <td> <a href="https://github.com/JuliaLang/julia/releases/download/v{{stable_release}}/julia-{{stable_release}}.tar.gz">Tarball</a>
        (<a href="https://github.com/JuliaLang/julia/releases/download/v{{stable_release}}/julia-{{stable_release}}.tar.gz.asc">GPG</a>)
      </td>
      <td> <a href="https://github.com/JuliaLang/julia/releases/download/v{{stable_release}}/julia-{{stable_release}}-full.tar.gz">Tarball with dependencies</a>
        (<a href="https://github.com/JuliaLang/julia/releases/download/v{{stable_release}}/julia-{{stable_release}}-full.tar.gz.asc">GPG</a>)
      </td>
      <td> <a href="https://github.com/JuliaLang/julia/tree/v{{stable_release}}">GitHub</a> </td>
    </tr>
  </tbody>
</table>
~~~
@@ @@

~~~
<div id="variant_builds_section" hidden>
<h3 id="variant_builds"><a href="#variant_builds">Optimized and assertion builds of v<span class="variant-version"></span></a></h3>
~~~

The same sources built differently: **optimized** builds use profile-guided optimization (PGO) and ThinLTO, and on Linux x86-64 and ARM also BOLT, which makes compilation and package loading faster; **assertion** builds enable Julia's and LLVM's internal checks, for debugging Julia itself. Install them with `juliaup add release+opt` (or `release+assert`), or download them below. See [the platform notes](/downloads/platform/#optimized_and_assertion_builds).

~~~
<p id="variant_builds_lagging" hidden>The optimized and assertion builds of a release are published some hours after it, platform by platform. Where a row below shows an older version, the newest release's build is not out yet for that platform, and <code>juliaup add release+opt</code> does not work there yet; the command in that row installs the listed version for that row's architecture instead.</p>
~~~

@@row @@col-12
~~~
<table class="downloads table table-hover table-bordered">
  <thead>
    <tr>
      <th> Platform</th>
      <th> Optimized</th>
      <th> Assertions</th>
    </tr>
  </thead>
  <tbody id="variant_builds_rows">
  </tbody>
</table>
</div>
<script>
  // Listed from versions.json, so that only builds that exist are linked: a
  // release's variants are published per platform, some hours after it.
  // versions.json lists a variant's tarball only; its other formats sit next to
  // it under the same name, and a platform is only promoted with all of them.
  (function () {
    var platforms = [
      ["winnt", "x86_64", "Windows (x86-64)"],
      ["mac", "aarch64", "macOS (Apple Silicon)"],
      ["mac", "x86_64", "macOS (Intel x86)"],
      ["linux", "x86_64", "Generic Linux on x86-64"],
      ["linux", "i686", "Generic Linux on x86 (32-bit)"],
      ["linux", "aarch64", "Generic Linux on ARM"]
    ];
    var variants = ["opt", "assert"];
    var labels = { exe: "installer", zip: "portable", dmg: ".dmg", "tar.gz": ".tar.gz" };
    var formats = { winnt: ["exe", "zip", "tar.gz"], mac: ["dmg", "tar.gz"], linux: ["tar.gz"] };
    // juliaup's names for the architectures, for channels like 1.14.0+opt~x86
    var juliaupArch = { x86_64: "x64", i686: "x86", aarch64: "aarch64" };

    function parse(version) {
      var m = /^(\d+)\.(\d+)\.(\d+)$/.exec(version);
      return m && [+m[1], +m[2], +m[3]];
    }

    function link(href, text) {
      var a = document.createElement("a");
      a.href = href;
      a.textContent = text;
      return a;
    }

    function cell(files, version, variant, newest, arch) {
      var td = document.createElement("td");
      var tarball = files.filter(function (file) { return file.extension === "tar.gz"; })[0];
      files = tarball ? formats[tarball.os].map(function (extension) {
        return { os: tarball.os, extension: extension, url: tarball.url.replace(/tar\.gz$/, extension) };
      }) : [];
      files.forEach(function (file, i) {
        if (i > 0) td.appendChild(document.createTextNode(", "));
        td.appendChild(link(file.url, labels[file.extension] || file.extension));
        if (file.extension === "tar.gz" && file.os === "linux") {
          td.appendChild(document.createTextNode(" ("));
          td.appendChild(link(file.url + ".asc", "GPG"));
          td.appendChild(document.createTextNode(")"));
        }
      });
      if (files.length && version !== newest) {
        var note = document.createElement("div");
        note.appendChild(document.createTextNode("v" + version + ": "));
        var code = document.createElement("code");
        code.textContent = "juliaup add " + version + "+" + variant + "~" + juliaupArch[arch];
        note.appendChild(code);
        td.appendChild(note);
      }
      return td;
    }

    fetch("https://julialang-s3.julialang.org/bin/versions.json")
      .then(function (response) { return response.json(); })
      .then(function (versions) {
        // The stable releases of the newest release series, newest first.
        var releases = Object.keys(versions)
          .filter(function (v) { return versions[v].stable && parse(v); })
          .sort(function (a, b) {
            var x = parse(a), y = parse(b);
            return y[0] - x[0] || y[1] - x[1] || y[2] - x[2];
          });
        if (!releases.length) return;
        var newest = releases[0];
        var series = parse(newest).slice(0, 2).join(".");
        releases = releases.filter(function (v) { return parse(v).slice(0, 2).join(".") === series; });

        var rows = document.getElementById("variant_builds_rows");
        var any = false, lagging = false;
        platforms.forEach(function (platform) {
          var tr = document.createElement("tr");
          var name = document.createElement("td");
          name.textContent = " " + platform[2];
          tr.appendChild(name);
          var listed = false;
          variants.forEach(function (variant) {
            // The newest release that has this variant for this platform.
            var version, files = [];
            for (var i = 0; i < releases.length && !files.length; i++) {
              version = releases[i];
              files = (versions[version].variants || []).filter(function (file) {
                return file.os === platform[0] && file.arch === platform[1] &&
                  (file.variants || []).indexOf(variant) !== -1;
              });
            }
            if (files.length) {
              listed = true;
              lagging = lagging || version !== newest;
            }
            tr.appendChild(cell(files, version, variant, newest, platform[1]));
          });
          if (listed) {
            rows.appendChild(tr);
            any = true;
          }
        });
        if (!any) return;
        document.querySelectorAll(".variant-version").forEach(function (el) { el.textContent = newest; });
        document.getElementById("variant_builds_lagging").hidden = !lagging;
        document.getElementById("variant_builds_section").hidden = false;
      })
      .catch(function (error) {
        console.error("Error listing the optimized and assertion builds:", error);
      });
  })();
</script>
~~~
@@ @@

Almost everyone should be downloading and using the latest stable release of Julia.
Great care is taken not to break compatibility with older Julia versions, so older code should continue to work with the latest stable Julia release.
You should *only* be using the long-term support (LTS) version of Julia if you work at an organization where implementing or certifying upgrades is prohibitively expensive and there is no need for new language features or packages. See this description of ["Risk Personas"](/blog/2019/08/release-process/#risk_tolerance_personas) for more detail on who should be using what versions of Julia based on their risk tolerance. See this blog post on [Julia's Release Process](/blog/2019/08/release-process/) for more information on different kinds of releases.

~~~
<br>
</div>

<div class="container-fluid alt-color packages">
  <br>
  <div class="container">
    <div class="row">
      <div class="col-lg-4 col-md-3 language-features"><hr/></div>
      <div class="col-lg-4 col-md-6 language-features section-heading">
        <h2 class="lead secondary-heading">Long-term Support Release</h2>
      </div>
      <div class="col-lg-4 col-md-3 language-features"><hr/></div>
    </div>
    <br>
~~~

~~~
<h3 id="long_term_support_release"><a href="#long_term_support_release">v{{lts_release}} ({{lts_release_date}})</a></h3>
~~~

[Release notes](https://github.com/JuliaLang/julia/blob/v{{lts_release}}/NEWS.md) | [GitHub tag](https://github.com/JuliaLang/julia/releases/tag/v{{lts_release}}) | [SHA256 checksums](https://julialang-s3.julialang.org/bin/checksums/julia-{{lts_release}}.sha256) | [MD5 checksums](https://julialang-s3.julialang.org/bin/checksums/julia-{{lts_release}}.md5)

@@row @@col-12
~~~
<table class="downloads table table-hover table-bordered">
  <tbody>
    <tr>
      <th> Platform</th>
      <th> 64-bit</th>
      <th> 32-bit</th>
    </tr>
    <tr>
      <td> Windows <a href="/downloads/platform/#windows">[help]</a></td>
      <td> <a href="https://julialang-s3.julialang.org/bin/winnt/x64/{{lts_release_short}}/julia-{{lts_release}}-win64.exe">installer</a>, <a href="https://julialang-s3.julialang.org/bin/winnt/x64/{{lts_release_short}}/julia-{{lts_release}}-win64.zip">portable</a> </td>
      <td> <a href="https://julialang-s3.julialang.org/bin/winnt/x86/{{lts_release_short}}/julia-{{lts_release}}-win32.exe">installer</a>,  <a href="https://julialang-s3.julialang.org/bin/winnt/x86/{{lts_release_short}}/julia-{{lts_release}}-win32.zip">portable</a> </td>
    </tr>
    <tr>
      <td> macOS (Apple Silicon) <a href="/downloads/platform/#macos">[help]</a></td>
      <td> <a href="https://julialang-s3.julialang.org/bin/mac/aarch64/{{lts_release_short}}/julia-{{lts_release}}-macaarch64.dmg">.dmg</a>, <a href="https://julialang-s3.julialang.org/bin/mac/aarch64/{{lts_release_short}}/julia-{{lts_release}}-macaarch64.tar.gz">.tar.gz</a> </td>
      <td> </td>
    </tr>
    <tr>
      <td> macOS (Intel x86) <a href="/downloads/platform/#macos">[help]</a></td>
      <td> <a href="https://julialang-s3.julialang.org/bin/mac/x64/{{lts_release_short}}/julia-{{lts_release}}-mac64.dmg">.dmg</a>, <a href="https://julialang-s3.julialang.org/bin/mac/x64/{{lts_release_short}}/julia-{{lts_release}}-mac64.tar.gz">.tar.gz</a> </td>
      <td> </td>
    </tr>
    <tr>
      <td> Generic Linux on x86 <a href="/downloads/platform/#linux_and_freebsd">[help]</a></td>
      <td>
        <a href="https://julialang-s3.julialang.org/bin/linux/x64/{{lts_release_short}}/julia-{{lts_release}}-linux-x86_64.tar.gz">glibc</a>
          (<a href="https://julialang-s3.julialang.org/bin/linux/x64/{{lts_release_short}}/julia-{{lts_release}}-linux-x86_64.tar.gz.asc">GPG</a>)<!--,
        <a href="https://julialang-s3.julialang.org/bin/musl/x64/{{lts_release_short}}/julia-{{lts_release}}-musl-x86_64.tar.gz">musl</a><sup>[<a href=#musl-fn>1</a>]</sup>
        (<a href="https://julialang-s3.julialang.org/bin/musl/x64/{{lts_release_short}}/julia-{{lts_release}}-musl-x86_64.tar.gz.asc">GPG</a>)-->
      </td>
      <td> <a href="https://julialang-s3.julialang.org/bin/linux/x86/{{lts_release_short}}/julia-{{lts_release}}-linux-i686.tar.gz">glibc</a>
        (<a href="https://julialang-s3.julialang.org/bin/linux/x86/{{lts_release_short}}/julia-{{lts_release}}-linux-i686.tar.gz.asc">GPG</a>)
      </td>
    </tr>
    <tr>
      <td> Generic Linux on ARM <a href="/downloads/platform/#linux_and_freebsd">[help]</a></td>
      <td> <a href="https://julialang-s3.julialang.org/bin/linux/aarch64/{{lts_release_short}}/julia-{{lts_release}}-linux-aarch64.tar.gz">.tar.gz</a>
          (<a href="https://julialang-s3.julialang.org/bin/linux/aarch64/{{lts_release_short}}/julia-{{lts_release}}-linux-aarch64.tar.gz.asc">GPG</a>)
      </td>
      <td> <!-- <a href="https://julialang-s3.julialang.org/bin/linux/armv7l/{{lts_release_short}}/julia-{{lts_release}}-linux-armv7l.tar.gz">ARMv7-a hard float</a>
          (<a href="https://julialang-s3.julialang.org/bin/linux/armv7l/{{lts_release_short}}/julia-{{lts_release}}-linux-armv7l.tar.gz.asc">GPG</a>) -->
      </td>
    </tr>
    <tr>
      <td> Generic Linux on PowerPC <a href="/downloads/platform/#linux_and_freebsd">[help]</a></td>
      <td> <a href="https://julialang-s3.julialang.org/bin/linux/ppc64le/{{lts_release_short}}/julia-{{lts_release}}-linux-ppc64le.tar.gz">little endian</a>
        (<a href="https://julialang-s3.julialang.org/bin/linux/ppc64le/{{lts_release_short}}/julia-{{lts_release}}-linux-ppc64le.tar.gz.asc">GPG</a>)
      </td>
      <td>
      </td>
    </tr>
    <tr>
      <td> Generic FreeBSD on x86 <a href="/downloads/platform/#linux_and_freebsd">[help]</a></td>
      <td> <a href="https://julialang-s3.julialang.org/bin/freebsd/x64/{{lts_release_short}}/julia-{{lts_release}}-freebsd-x86_64.tar.gz">.tar.gz</a>
          (<a href="https://julialang-s3.julialang.org/bin/freebsd/x64/{{lts_release_short}}/julia-{{lts_release}}-freebsd-x86_64.tar.gz.asc">GPG</a>)
      </td>
      <td> </td>
    </tr>
  </tbody>
</table>
<table>
  <tbody>
    <tr>
      <th> Source </th>
      <td> <a href="https://github.com/JuliaLang/julia/releases/download/v{{lts_release}}/julia-{{lts_release}}.tar.gz">Tarball</a>
            (<a href="https://github.com/JuliaLang/julia/releases/download/v{{lts_release}}/julia-{{lts_release}}.tar.gz.asc">GPG</a>)
      </td>
      <td> <a href="https://github.com/JuliaLang/julia/releases/download/v{{lts_release}}/julia-{{lts_release}}-full.tar.gz">Tarball with dependencies</a>
        (<a href="https://github.com/JuliaLang/julia/releases/download/v{{lts_release}}/julia-{{lts_release}}-full.tar.gz.asc">GPG</a>)
      </td>
      <td> <a href="https://github.com/JuliaLang/julia/tree/v{{lts_release}}">GitHub</a> </td>
    </tr>
  </tbody>
</table>
~~~
@@ @@

~~~
    <br>
  </div>
</div>
~~~

{{ifdef upcoming_release}}

~~~
<div class="container pt-sm-2">
  <div class="row">
    <div class="col-lg-4 col-md-3 language-features"><hr/></div>
    <div class="col-lg-4 col-md-6 language-features section-heading">
      <h2 class="lead secondary-heading">Upcoming Release</h2>
    </div>
    <div class="col-lg-4 col-md-3 language-features"><hr/></div>
  </div>
  <br>
~~~

We're currently testing a prerelease for Julia v{{upcoming_release_short}}, an upcoming minor release in the 1.x series of releases. We encourage developers and interested users to try it out and report any issues they encounter. As a prerelease, it should not be considered production-ready; it's intended to give users a chance to try out {{upcoming_release_short}} with their code before the full release.

~~~
<h3 id="upcoming_release"><a href="#upcoming_release">v{{upcoming_release}} ({{upcoming_release_date}})</a></h3>
~~~

[Release notes](https://github.com/JuliaLang/julia/blob/v{{upcoming_release}}/NEWS.md) | [GitHub tag](https://github.com/JuliaLang/julia/releases/tag/v{{upcoming_release}}) | [SHA256 checksums](https://julialang-s3.julialang.org/bin/checksums/julia-{{upcoming_release}}.sha256) | [MD5 checksums](https://julialang-s3.julialang.org/bin/checksums/julia-{{upcoming_release}}.md5)

@@row @@col-12
~~~
<table class="downloads table table-hover  table-bordered">
  <tbody>
    <tr>
      <th> Platform</th>
      <th> 64-bit</th>
      <th> 32-bit</th>
    </tr>
    <tr>
      <td> Windows <a href="/downloads/platform/#windows">[help]</a></td>
      <td> <a href="https://julialang-s3.julialang.org/bin/winnt/x64/{{upcoming_release_short}}/julia-{{upcoming_release}}-win64.exe">installer</a>, <a href="https://julialang-s3.julialang.org/bin/winnt/x64/{{upcoming_release_short}}/julia-{{upcoming_release}}-win64.zip">portable</a> </td>
      <td> <a href="https://julialang-s3.julialang.org/bin/winnt/x86/{{upcoming_release_short}}/julia-{{upcoming_release}}-win32.exe">installer</a>,  <a href="https://julialang-s3.julialang.org/bin/winnt/x86/{{upcoming_release_short}}/julia-{{upcoming_release}}-win32.zip">portable</a> </td>
    </tr>
    <tr>
      <td> macOS (Intel x86) <a href="/downloads/platform/#macos">[help]</a></td>
      <td> <a href="https://julialang-s3.julialang.org/bin/mac/x64/{{upcoming_release_short}}/julia-{{upcoming_release}}-mac64.dmg">.dmg</a> </td>
      <td> </td>
    </tr>
    <tr>
      <td> macOS (Apple Silicon) <a href="/downloads/platform/#macos">[help]</a></td>
      <td> <a href="https://julialang-s3.julialang.org/bin/mac/aarch64/{{upcoming_release_short}}/julia-{{upcoming_release}}-macaarch64.dmg">.dmg</a> </td>
      <td> </td>
    </tr>
    <tr>
      <td> Generic Linux on x86 <a href="/downloads/platform/#linux_and_freebsd">[help]</a></td>
      <td>
        <a href="https://julialang-s3.julialang.org/bin/linux/x64/{{upcoming_release_short}}/julia-{{upcoming_release}}-linux-x86_64.tar.gz">glibc</a>
        (<a href="https://julialang-s3.julialang.org/bin/linux/x64/{{upcoming_release_short}}/julia-{{upcoming_release}}-linux-x86_64.tar.gz.asc">GPG</a>)<!--,
        <a href="https://julialang-s3.julialang.org/bin/musl/x64/{{upcoming_release_short}}/julia-{{upcoming_release}}-musl-x86_64.tar.gz">musl</a><sup>[<a href=#musl-fn>1</a>]</sup>
        (<a href="https://julialang-s3.julialang.org/bin/musl/x64/{{upcoming_release_short}}/julia-{{upcoming_release}}-musl-x86_64.tar.gz.asc">GPG</a>)-->
      </td>
      <td> <a href="https://julialang-s3.julialang.org/bin/linux/x86/{{upcoming_release_short}}/julia-{{upcoming_release}}-linux-i686.tar.gz">glibc</a>
        (<a href="https://julialang-s3.julialang.org/bin/linux/x86/{{upcoming_release_short}}/julia-{{upcoming_release}}-linux-i686.tar.gz.asc">GPG</a>)
      </td>
    </tr>
    <tr>
      <td> Generic Linux on ARM <a href="/downloads/platform/#linux_and_freebsd">[help]</a></td>
      <td> <a href="https://julialang-s3.julialang.org/bin/linux/aarch64/{{upcoming_release_short}}/julia-{{upcoming_release}}-linux-aarch64.tar.gz">AArch64</a>
        (<a href="https://julialang-s3.julialang.org/bin/linux/aarch64/{{upcoming_release_short}}/julia-{{upcoming_release}}-linux-aarch64.tar.gz.asc">GPG</a>)
      </td>
      <td> <!-- <a href="https://julialang-s3.julialang.org/bin/linux/armv7l/{{upcoming_release_short}}/julia-{{upcoming_release}}-linux-armv7l.tar.gz">ARMv7-a hard float</a>
                                       (<a href="https://julialang-s3.julialang.org/bin/linux/armv7l/{{upcoming_release_short}}/julia-{{upcoming_release}}-linux-armv7l.tar.gz.asc">GPG</a>) -->
      </td>
    </tr>
    <!--
    <tr>
      <td> Generic Linux on PowerPC <a href="/downloads/platform/#linux_and_freebsd">[help]</a></td>
      <td> <a href="https://julialang-s3.julialang.org/bin/linux/ppc64le/{{upcoming_release_short}}/julia-{{upcoming_release}}-linux-ppc64le.tar.gz">little endian</a>
        (<a href="https://julialang-s3.julialang.org/bin/linux/ppc64le/{{upcoming_release_short}}/julia-{{upcoming_release}}-linux-ppc64le.tar.gz.asc">GPG</a>)
      </td>
      <td>
      </td>
    </tr>
    -->
    <tr>
      <td> Generic FreeBSD on x86 <a href="/downloads/platform/#linux_and_freebsd">[help]</a></td>
      <td> <a href="https://julialang-s3.julialang.org/bin/freebsd/x64/{{upcoming_release_short}}/julia-{{upcoming_release}}-freebsd-x86_64.tar.gz">.tar.gz</a>
        (<a href="https://julialang-s3.julialang.org/bin/freebsd/x64/{{upcoming_release_short}}/julia-{{upcoming_release}}-freebsd-x86_64.tar.gz.asc">GPG</a>)
      </td>
      <td> </td>
    </tr>
  </tbody>
</table>
<table>
  <tbody>
    <tr>
      <th> Source </th>
      <td> <a href="https://github.com/JuliaLang/julia/releases/download/v{{upcoming_release}}/julia-{{upcoming_release}}.tar.gz">Tarball</a>
        (<a href="https://github.com/JuliaLang/julia/releases/download/v{{upcoming_release}}/julia-{{upcoming_release}}.tar.gz.asc">GPG</a>)
      </td>
      <td> <a href="https://github.com/JuliaLang/julia/releases/download/v{{upcoming_release}}/julia-{{upcoming_release}}-full.tar.gz">Tarball with dependencies</a>
        (<a href="https://github.com/JuliaLang/julia/releases/download/v{{upcoming_release}}/julia-{{upcoming_release}}-full.tar.gz.asc">GPG</a>)
      </td>
      <td> <a href="https://github.com/JuliaLang/julia/tree/v{{upcoming_release}}">GitHub</a> </td>
    </tr>
  </tbody>
</table>
~~~
@@ @@

<!-- NOTE: Uncomment this if/when any of the musl links above get uncommented
\label{musl-fn}
~~~
<sup>[1]</sup>
~~~
Most Linux users should use the glibc binaries unless you know that your system uses musl as its libc.
-->

~~~
<br>
</div>
~~~

{{end}} <!-- upcoming_release -->

~~~
<div class="container-fluid alt-color packages">
  <br>
  <div class="container">
    <div class="row">
      <div class="col-lg-4 col-md-3 language-features"><hr/></div>
      <div class="col-lg-4 col-md-6 language-features section-heading">
        <h2 class="lead secondary-heading">Supported Platforms</h2>
      </div>
      <div class="col-lg-4 col-md-3 language-features"><hr/></div>
    </div>
    <br>
~~~

Julia supports all the major operating systems, but specific versions and architectures have different [tiers of support](/downloads/support).

Please do not use Julia shipped by Linux or BSD package managers. Many Linux/BSD/Unix package managers ship broken and/or significantly out of date versions of Julia. Please use [`juliaup`](/downloads) or download the official binaries instead.

~~~
    <br>
  </div>
</div>

<div class="container pt-sm-2">
  <div class="row">
    <div class="col-lg-4 col-md-3 language-features"><hr/></div>
    <div class="col-lg-4 col-md-6 language-features section-heading">
      <h2 class="lead secondary-heading">Additional Resources</h2>
    </div>
    <div class="col-lg-4 col-md-3 language-features"><hr/></div>
  </div>
  <br>
~~~

**Older Releases** — Older releases of Julia for all platforms are available on the [Older releases page](/downloads/oldreleases/). Only the LTS and Stable releases are maintained.

**Nightly Builds** — Builds of the current unstable development version of Julia are available on the [nightlies page](/downloads/nightlies/). While the name suggests that they are built every night, they are actually built after each commit to master. However, at times due to broken builds or CI infrastructure issues, nightlies may not be produced. These are intended as developer previews into the latest work and are not intended for normal use. Most users are advised to use the current stable release version of Julia.

**Download verification** — All Julia binary releases are cryptographically secured using the traditional methods on each platform. macOS and Windows releases are codesigned with certificates that are verified by the operating system during installation. Linux and source tarballs are signed with GPG using [this key](/assets/juliareleases.asc). As of August 2026 (starting with v1.13.0-rc2), releases are signed with the key whose fingerprint is `64B779A570972FFF7BFC2B54EAD471E1A1F2C10A`. The previous signing key (fingerprint `3673DF529D9049477F76B37566E3C7DC03D6E495`) has been retired and should no longer be trusted; signatures made with it should not be relied upon.

**JSON release feed** — The info above is also available as a [JSON file](https://julialang-s3.julialang.org/bin/versions.json) ([schema](https://julialang-s3.julialang.org/bin/versions-schema.json)). It may take up to two hours after the release of a new version for it to be included in the JSON file.

~~~
<br>
</div>
~~~
