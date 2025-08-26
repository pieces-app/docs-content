---
title: Pieces Drive
path: /extensions-plugins/jetbrains/drive
visibility: PUBLIC
status: PUBLISHED
description: Snippets are useful pieces of code you can save, share, reuse, and modify to boost productivity and save time.
metaTitle: Using Pieces Drive in JetBrains | Pieces Docs
metaDescription: With the Pieces for JetBrains Plugin, you can save all kinds of code snippets, and easily find them and edit them whenever, wherever, and however you need.
---

## Using Pieces Drive in JetBrains

With the <a target="_blank" href="https://plugins.jetbrains.com/plugin/17328-pieces">Pieces for JetBrains Plugin</a>, you can save all kinds of code snippets and easily find [them](/products/extensions-plugins/jetbrains/drive/edit-update#how-to-edit-snippets) whenever, wherever, and however you need.

Let’s take a look at some examples:

***

| `SQL Query Templates`        | An SQL query to retrieve data from a database with filter conditions.                         | Save time with databases by reusing common queries like inserts, updates, or data retrieval.                |
| ---------------------------- | --------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| `Boilerplate Code`           | An HTML boilerplate template for creating new webpages.                                       | Standardize the project structure of different projects by starting with a clean and organized template.    |
| `Error-Handling Code Blocks` | A try-catch block template in JavaScript for handling API call errors.                        | Streamline error management by quickly inserting predefined error-handling patterns for more reliable code. |
| `Regex Patterns`             | A regex pattern to validate email addresses.                                                  | Quickly implement validation in forms to make sure users correctly enter formatted data.                    |
| `Shell Scripts`              | A shell script to automate server maintenance tasks like clearing logs and updating packages. | Automate system administration tasks on Unix / Linux servers so you spend less time on manual upkeep.       |

***

## Streamlining Development with Snippet Management

The <a target="_blank" href="https://plugins.jetbrains.com/plugin/17328-pieces">Pieces for JetBrains Plugin</a> connects you with your development environment, allowing you to focus on what matters—building great software—while empowering you with tools for efficient code reuse.

* **Improved Productivity:** Focus on solving new problems rather than resolving old ones.

* **Contextual Awareness:** Snippets enriched with metadata, descriptions, and links to relevant searches help you remember each piece of code's origin, purpose, and ideal usage scenarios.

* **Code Standardization:** Sharing best practices and reusable components helps developers ensure uniform coding practices and conventions are available across different teams and projects.

By using the <a target="_blank" href="https://plugins.jetbrains.com/plugin/17328-pieces">Pieces for JetBrains Plugin</a>, you can capture and manage these snippets to streamline daily tasks and enhance your workflow in several ways:

### Save & Organize

Users can save snippets by highlighting the desired code, right-clicking, and selecting the `Save to Pieces` option.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/using_snippets/MAIN_using_snippets/save_to_pieces.gif" alt="" align="center" fullwidth="true" />

You can also do this without opening the right-click menu—use the `⌥+⌘+p` (macOS) or `ctrl+shift+p` (Windows/Linux) shortcut while your code is highlighted.

This guarantees that essential pieces of code, such as code fragments, functions, configuration files, and command-line instructions, are always at hand when needed.

Additionally, [each snippet is enriched with context](/products/extensions-plugins/jetbrains/drive/save-snippets#what-happens-when-you-save-a-snippet), enabling you to insert well-documented, relevant snippets where they make sense within your projects.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/using_snippets/MAIN_using_snippets/snippet_enrichment.png" alt="" align="center" fullwidth="true" />

Pieces can also intelligently identify and save snippets based on re-use patterns in your JetBrains workflow.

Whenever Pieces saves a snippet, you'll see a confirmation in the bottom right corner of your screen that says `Snippet Successfully Saved to Pieces`.

Your snippet is now saved in Pieces Drive with auto-generated metadata!

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/using_snippets/MAIN_using_snippets/opening_snippet.gif" alt="" align="center" fullwidth="true" />

### Search & Reuse

You can [search your entire collection of saved Pieces code snippets](/products/extensions-plugins/jetbrains/drive/search-reuse) inside of your preferred JetBrains IDE, so the code you need is always on hand.

To do this, open the **Search Everywhere** window and switch to the `Pieces` tab by using `⌘+shift+p` (macOS) or `ctrl+shift+p` (Windows/Linux).

Enter a search query, and any related snippets will appear in the dropdown list—then you can hit enter and view your snippet (with all of its saved context) rendered in markdown directly inside your editor.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/using_snippets/MAIN_using_snippets/opening_pieces_command_pallete.gif" alt="" align="center" fullwidth="true" />

### Edit & Update

You can easily [edit and update code snippets](/products/extensions-plugins/jetbrains/drive/edit-update#how-to-edit-snippets) directly from your IDE without opening a separate window or navigating to the Pieces for Developers Desktop App.

To do so, open the **Pieces** from the tool window on the left-hand side of your JetBrains IDE, revealing a list of saved snippets. You can then right-click a snippet, which opens that snippet up in a new window.

Make changes and save the snippet using `⌘+s` (macOS) or `ctrl+s` (Windows/Linux).

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/using_snippets/MAIN_using_snippets/editing_snippet.gif" alt="" align="center" fullwidth="true" />

### Sharing

The **Sharing Snippets** feature allows you to [share code snippets with your team](/products/extensions-plugins/jetbrains/drive/sharing) or across projects directly from your JetBrains IDE.

To share a snippet, right-click on some highlighted code, hover over the Pieces option, and select `Share via Pieces Link`.

You can also share a snippet by right-clicking a snippet that’s listed in the left-hand toolbar window in any of your JetBrains IDEs and clicking `Share via Pieces Link`**.**

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/using_snippets/MAIN_using_snippets/share_via_pieces_link.gif" alt="" align="center" fullwidth="true" />

## Use Cases

With Pieces for JetBrains Plugin, your snippets become a robust library of reusable code that you can organize, search, edit, and share across projects.

Here are some examples of how you can use them:

### Reusable Scheduling Functions

Imagine you’re frequently working on projects that involve scheduling tasks at regular intervals.

Instead of rewriting the same logic for each new project, you can [save an evergreen snippet to your Pieces repository.](/products/extensions-plugins/jetbrains/drive/save-snippets#saving-snippets)

This allows you to reuse a well-crafted scheduling function across multiple applications, that is useful in a variety of scenarios:

```go
package main

import (
	"fmt"
	"time"
)

// A reusable function to schedule tasks at a specified interval
func scheduleTask(interval time.Duration, task func()) {
	ticker := time.NewTicker(interval)
	defer ticker.Stop()

	for {
		select {
		case <-ticker.C:
			task()
		}
	}
}
```

### File System Monitoring

Suppose you frequently work on projects that involve monitoring file system changes. In that case, you can [save a helpful snippet to your Pieces Drive](/products/extensions-plugins/jetbrains/drive/save-snippets#saving-snippets) that does precisely that, using generic and reusable naming conventions:

```go
package main

import (
	"fmt"
	"log"
	"github.com/fsnotify/fsnotify"
)

// A reusable function to monitor file system changes
func watchFileChanges(path string) {
	watcher, err := fsnotify.NewWatcher()
	if err != nil {
		log.Fatal(err)
	}
	defer watcher.Close()

	err = watcher.Add(path)
	if err != nil {
		log.Fatal(err)
	}

	for {
		select {
		case event := <-watcher.Events:
			if event.Op&fsnotify.Write == fsnotify.Write {
				fmt.Println("Modified file:", event.Name)
			}
		case err := <-watcher.Errors:
			fmt.Println("Error:", err)
		}
	}
}
```

## Additional Snippet Scenarios

Review some additional scenarios and use cases for Pieces Snippets and see how the <a target="_blank" href="https://plugins.jetbrains.com/plugin/17328-pieces">Pieces for JetBrains Plugin</a> could benefit you and your workflow.

***

<AccordionGroup>
  <Accordion title="Project Initialization">
    Quickly set up new projects by reusing boilerplate code.

    Save standard project initialization scripts, configuration files, and setup commands as snippets to ensure consistency and save time when starting a new project.
  </Accordion>

  <Accordion title="Common Functions and Utilities">
    Reuse frequently used functions and utility methods by saving snippets of commonly used functions, such as data validation methods, API request handlers, or utility functions.

    This allows you to quickly insert these snippets into new projects without rewriting them.
  </Accordion>

  <Accordion title="Configuration Management">
    Save snippets of configuration files for development, testing, and production to manage and reuse configuration files across different environments.
  </Accordion>

  <Accordion title="Documentation and Learning">
    Create a library of well-documented code examples for learning and reference by saving snippets with detailed descriptions and metadata.

    This personal or team library of code examples makes learning new concepts easier and referencing how specific tasks were previously accomplished.
  </Accordion>

  <Accordion title="Command-Line Instructions">
    Store complicated command-line instructions as a code snippet so that you don’t need to remember the syntax every time you need to use a specific command-line instruction.
  </Accordion>

  <Accordion title="Bug Fixes and Patches">
    Save and reuse bug fixes or patches by storing the fix as a snippet when you solve a common bug or issue.

    This allows you to quickly apply the same fix in other projects or share it with team members who might encounter the same issue.
  </Accordion>
</AccordionGroup>

***

<a target="_blank" href="/products/extensions-plugins/jetbrains/get-started">Download the Pieces for JetBrains Plugin today!</a>