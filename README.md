# How to Process a `boot.img` Using GitHub Actions

This tutorial will guide you through the steps to process a `boot.img` file using a GitHub Action. The workflow will download the `boot.img`, extract information about the kernel format, and save the output to a file.

## Step 1: Fork the Repository

1. **Fork the Repository**:  
   In the top-right corner of the page, click the **Fork** button. This creates a copy of the repository under your GitHub account.

## Step 2: Upload Your `boot.img` File

1. **Prepare Your `boot.img`**:  
   You will need to upload a `boot.img` file for processing. Ensure your `boot.img` file is correctly named `boot.img` (all lowercase).

2. **Upload `boot.img` to Your Fork**:
   - https://filebin.net/
   - Click on the **Add file** button and select **Upload files**.

## Step 3: Enter URL and Run the Action

1. **Navigate to the Actions Tab**:
   - Go to the **Actions** tab in your forked repository.  
   - This tab lists all workflows in the repository. Find the workflow designed to process the `boot.img`.

2. **Run the Action**:
   - In the Actions tab, locate the workflow named **"Process boot.img from URL"** or similar.
   - Click on the workflow and press the **Run workflow** button.
   - Enter the URL to the `boot.img` file you uploaded in Step 2.
     - You can use the raw URL of the `boot.img`. The URL should look something like:  
       `https://filebin.net/gp05fto9lulm3qwg/boot.img`
   - Click **Run workflow** to trigger the GitHub Action.

## Step 4: View Kernel Format from the Action's Output

1. **Wait for the Action to Complete**:
   - The workflow will begin processing. This includes downloading the `boot.img` file, extracting kernel format information.
   - Wait for the action to finish. You can monitor the progress from the GitHub Actions interface.

2. **Check the Output**:
   - Once the action completes, view the **logs** from the workflow run.
   - You’ll see the kernel format (`KERNEL_FMT`) printed in the logs.

## Summary

You’ve now successfully processed a `boot.img` file using GitHub Actions:

- Forked the repo.
- Uploaded the `boot.img` file.
- Ran the GitHub Action to process it.
- Retrieved the kernel format.
