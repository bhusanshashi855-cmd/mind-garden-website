# 🌱 Mind Garden

Project link - https://dancing-maamoul-39afdd.netlify.app/

**Plant your ideas, watch them grow.**

Mind Garden is a simple, friendly website for saving your ideas and watching them grow. Every idea starts as a seed in your garden. Add a to-do list to each idea, and every task you finish grows the plant from a seed to a sprout to a full sunflower.

Built with plain HTML, CSS and JavaScript. No frameworks, no build step, no installation.

## Table of contents

- [Features](#features)
- [How growth works](#how-growth-works)
- [How to run it](#how-to-run-it)
- [Project structure](#project-structure)
- [Saving your data](#saving-your-data)
- [Fonts](#fonts)
- [Ideas for the future](#ideas-for-the-future)
- [License](#license)

## Features

- **Landing page** with the project name, tagline, a short description and a "Plant an idea" button
- **Your plants** section on the home page showing each idea with its plant, the reason behind it and its progress
- **Plant an idea** form: idea name, short description, category and why the idea is useful
- **Garden** where every idea is a plant growing in its own little scene
- **Idea details** with the description, category, reason, current stage and a progress bar
- **To-do list for each idea:** add, edit, delete and tick off tasks
- **View all to-do's** button to see every task for an idea in one window
- **Automatic progress** based on completed tasks
- **Growing plants** that change as progress increases, with a petal celebration at 100%
- **Saved in your browser** so your garden is still there when you come back
- **Responsive** layout for phones and computers

## How growth works

Progress is the share of completed tasks, and it updates the moment you tick or untick a task.

| Tasks completed | Progress |
| --------------- | -------- |
| 0 of 4          | 0%       |
| 2 of 4          | 50%      |
| 4 of 4          | 100%     |

The plant stage follows the progress:

| Progress  | Stage   |
| --------- | ------- |
| 0–24%     | Seed    |
| 25–49%    | Sprout  |
| 50–99%    | Growing |
| 100%      | Mature  |

An idea with no tasks stays at 0%.

## How to run it

1. Download or clone this repository.
2. Open `index.html` in your web browser.

That's all. You can also host it for free with GitHub Pages or Netlify, and it will work the same way.

## Project structure

```
mind-garden/
├── index.html   # Page structure: home, garden and the pop-up windows
├── style.css    # All styling, including the scene and animations
├── script.js    # All behaviour: ideas, tasks, progress and plant drawings
└── README.md
```

Where to change things:

- **Plant drawings:** the `plantSVG()` function in `script.js`
- **Stage thresholds:** the `stageOf()` function in `script.js`
- **Colors and fonts:** the variables at the top of `style.css` and the sections at the bottom
- **Sky, sun and hills:** the SVG at the top of `index.html`

## Saving your data

Ideas and tasks are saved in your browser's local storage, under the key `mindGardenIdeas`. This means:

- Your garden stays after you refresh or close the page.
- It is private to that browser on that device. It won't appear on another phone or computer.
- Clearing your browser's site data will delete your ideas.

## Fonts

The page loads the Fredoka and Playfair Display fonts from Google Fonts. If you are offline, it falls back to standard system fonts and still works.

## Ideas for the future

- Edit an idea after planting it
- Search and filter by category or stage
- Different flowers for different categories
- Download and restore a backup of your garden
- Due dates for tasks
- Day and night mode

## License

Add a license of your choice here (for example MIT) before sharing the project publicly.
