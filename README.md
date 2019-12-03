# git-lfs-initialize-buildkite-plugin

For when the git-lfs binaries are installed on your agents, but `git lfs install` hasn't been run
yet, so buildkite's git clone doesn't have your lfs'd binaries.

Whack this plugin in your pipeline and hey presto, initial clones correctly smudge the refernce
files into the binaries they represent.

## Usage

In your `buildkite.yml` pipeline definition:

```yaml
plugins:
  envato/git-lfs-initialize#9a3d82b1fed2951156e396e5e10abb23a6d80fd3:
    there_is: no_config
```
