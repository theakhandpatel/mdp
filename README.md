# Markdown Previewer
This is a simple tool to preview markdown files. It converts markdown files into HTML and provides a preview of the rendered content.

## Building the Project
To build the project, you need to have Go installed on your machine. Once you have Go installed, you can build the project using the following command:
```bash
go build -o mdp main.go
```
This will create an executable named mdp in your current directory.

## Running the Project
To run the project, you can use the following command:
```bash
./mdp -file your_markdown_file.md
```
Replace your_markdown_file.md with the path to the markdown file you want to preview.

## Auto Preview
The autopreview.sh script is provided to automatically preview the changes to the markdown file. It checks for changes to the specified file every 5 seconds and runs the mdp tool if any changes are detected.

To use the auto preview feature, you need to have md5sum installed on your machine. Once you have md5sum installed, you can start the auto preview using the following command:
```bash
./autopreview.sh your_markdown_file.md
```
Replace your_markdown_file.md with the path to the markdown file you want to auto preview.

## Customizing the HTML Template
You can customize the HTML template used to render the markdown by providing an alternative template file using the -t flag:
```bash
./mdp -file your_markdown_file.md -t your_template_file.tmpl
```
Replace your_template_file.tmpl with the path to your custom template file.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```