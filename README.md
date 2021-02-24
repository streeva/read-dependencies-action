# Read Dependencies
This parses application manifest files to extract a list of dependencies.

Currently only supports NuGet for C#, by default it will walk the directory tree from the workspace directory and parse any csproj files it finds for PackageReference entries, but it can be directed to a specific file, any dependencies it reads are written to a file in CSV format. This intermediate format can then be used as the source for some companion utilities which will do things such as creating reports or checking and reporting any known security vulnerabilities.

# Usage

See [action.yml](action.yml)