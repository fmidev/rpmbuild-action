# GitHub Action - RPM Build  

This GitHub Action builds RPMs from spec file and using repository contents as source (wraps the rpmbuild utility).

Inspired by naveenrajm7/rpmbuild@master.

## Usage

### Inputs

- `spec_file`: The path to the spec file in your repo. [**required**]
- `additional_repos`: A list of additional repositories that you want enabled [**optional**]
- `enable_modules`: A list of dnf modules to enable [**optional**]
- `disable_modules`: A list of dnf modules to disable [**optional**]
- `dnf_commands`: Command that's executed as a part of the package initialization [**optional**]
- `pre_build_hook`: Command that's execute before rpm build starts [**optional**]
- `post_build_hook`: Command that's execute after rpm build is finished [**optional**]

### Outputs

- `rpm_dir_path`: path to RPMS directory
- `srpm_dir_path`: path to SRPMS directory

### Example workflow - build RPM

https://github.com/fmidev/github-actions-workflows/blob/main/.github/workflows/rpmbuild-workflow.yaml


