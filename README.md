# MTI Digital Garden

Live website: [https://jonfelix1.github.io/mti-quartz/](https://jonfelix1.github.io/mti-quartz/)

## Repository Structure

All notes are stored in the `contents/` directory. They are divided into different courses.

## Local Setup

### Prerequisites
Make sure you have the following installed before proceeding:

- **NodeJS** v18.14+ (check your version using `node -v`)
- **NPM** v9.3.1+ (check your version using `npm -v`)
- **Git** (check your version using `git --version`)
- **Obsidian**

### Initial Setup

1. Clone this repository:
    ```bash
    git clone git@github.com:jonfelix1/mti-quartz.git
    ```

2. Change directory to this repository:
    ```bash
    cd mti-quartz
    ```

3. Install dependencies using NPM:
    ```bash
    npm i
    ```

4. Set up Obsidian: Open Obsidian and use this repo as a vault. All files will be in the `contents` directory.

5. Serve the website locally:
    ```bash
    npx quartz build --serve
    ```
    The website will run at `http://localhost:8080`.

## Contribution

Feel free to open a pull request to contribute to this project. Follow the standard [GitHub Workflow](https://gist.github.com/Chaser324/ce0505fbed06b947d962).

Please adhere to the tagging conventions used in the surrounding notes by linking them to the respective topic index. Ensure each note is appropriately tagged.