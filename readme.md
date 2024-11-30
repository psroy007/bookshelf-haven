# Bookshelf Haven - An Environment For Story Readers and Writers

A simple web-based story collection application that allows users to upload, view, edit, and delete stories. The stories are stored locally in the browser's `localStorage`, and users can upload text or document files, view their descriptions, and even download the uploaded content. This project is designed for educational purposes and demonstrates file handling in JavaScript with a focus on local storage and dynamic content display.

## Features

- **Story Upload**: Users can upload stories with a title, description, and a file (text or document).
- **Story Display**: Uploaded stories are displayed with their title and description.
- **Story Editing**: Users can edit the title and description of a story.
- **Story Deletion**: Users can delete a story from the collection.
- **Download Support**: Uploaded files (stored as Base64) can be downloaded again from the app.
- **Responsive Design**: The app works on both desktop and mobile devices.

## Technologies Used

- **HTML**: For structuring the content of the page.
- **CSS**: For styling the page and ensuring a responsive design.
- **JavaScript**: For handling story uploads, editing, deletion, and local storage interaction.
- **localStorage**: For storing stories persistently in the user's browser.

## Getting Started

To run this project locally, follow these steps:

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, etc.) with support for `localStorage`.

### Running the Project

1. Clone this repository:
    ```bash
    git clone https://github.com/psroy007/bookshelf-haven.git
    ```
2. Open the `index.html` file in your browser to view the app.

### How the App Works

- **Uploading Stories**: 
  - Click on the "Upload Your Story" form and enter a title, description, and upload a story file (text or document).
  - The file will be encoded in Base64 and stored in `localStorage`.
  
- **Viewing Stories**:
  - After uploading a story, it will appear in the main content area with its title and description.
  - Click "Read more" to view the story's content (Base64 encoded). The content can be downloaded using a dynamic link.

- **Editing Stories**(only available for admin/developer):
  - Click the "Edit" button next to a story to update its title or description. The old story is removed from `localStorage`, and the new story is saved.

- **Deleting Stories**(only available for admin/developer):
  - Click the "Delete" button next to a story to remove it from `localStorage`.

### Features in Detail

- **Story Upload Form**: 
  The upload form allows the user to select a file (`.txt`, `.docx`, `.pdf`) and adds the content to the `localStorage` in Base64 format.

- **Story Display**:
  Each uploaded story is displayed with its title and description. The story content is stored as a Base64 encoded string.

- **Read More**:
  Clicking "Read More" displays the story content in an alert and allows the user to download the file.

- **Responsive Design**:
  The app is designed to work well on both desktop and mobile devices. It adjusts the layout for smaller screens to ensure a smooth user experience.

### Main JavaScript Functions:

- **displayStories()**: Displays all stories stored in `localStorage`.
- **viewStory(index)**: Displays the full content of a selected story and allows the user to download it.
- **editStory(index)**: Allows the user to edit the title and description of a story.
- **deleteStory(index)**: Deletes the selected story from `localStorage`.
- **handleFormSubmit(event)**: Handles the form submission, processes the uploaded file, and stores the story in `localStorage`.

## Future Improvements

- Implement a file format checker to validate uploaded files.
- Add user authentication to allow saving stories across multiple devices.
- Allow users to edit the content of the uploaded file, not just the title and description.
- Enhance the UI/UX with better styling and dynamic page transitions.

## Acknowledgments

- The project is built with basic front-end technologies to demonstrate the power of `localStorage` for persistent data storage in the browser.
- Inspiration for the design and layout was derived from various UI patterns available online.

## Contact

- **Purab Singha Roy** - [purabsingharoy90@gmail.com](mailto:purabsingharoy90@gmail.com)
- GitHub: [https://github.com/psroy007](https://github.com/psroy007)
