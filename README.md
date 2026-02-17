# Release Magisk Module Workflow Template
Simple workflow that release module to GitHub release channel

This template provides an automated GitHub Actions workflow for Magisk module developers to easily release and update their modules through GitHub Releases.

## Features

- Automated versioning and release creation
- Automated zip file creation and upload
- Simple integration with existing Magisk module projects

## Setup Instructions

### 1. Create a new repository using this template

Click the "Use this template" button to create a new repository based on this workflow template.

### 2. Configure GitHub Actions permissions

Enable GitHub Actions in your repository settings and ensure it has read and write permissions:

1. Go to your repository **Settings**
2. Navigate to **Actions > General** 
3. Under "Workflow permissions", select **"Read and write permissions"**
4. Save your changes

### 3. Customize your module files

- Add your Magisk module files to the repository in module directory
- Update `update.json` with your repository information
- Create initial module version in `changelog.md`

## Usage

### Creating a new release

1. Make changes to your module files
2. Update version information in `update.json` and `module.prop` 
3. Add new version details to `changelog.md`
4. Commit and push your changes
5. Start workflow
6. The workflow will automatically:
   - Create a zip file of your module
   - Create a GitHub release with your specified version
   
### Configuration options

You can customize the workflow behavior by modifying the `.github/workflows/release.yml` file according to your specific needs.

## File Structure

- `update.json` - Module update information (version, download URL)
- `changelog.md` - Version history and changes
- `module.prop` - Module properties and metadata
- `module` - Directory containing your Magisk module files
- `LICENSE` - MIT License for this template

## License

This template is released under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
