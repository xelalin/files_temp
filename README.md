# Vivado AI Assistant Environment setup 
### Set up the Vivado AI Assistant toolchain in your Windows OS environment. Each guide walks you through installation, configuration, and a first test to verify everything works.
## Step 0 : Prerequisites
- Request access to the [AMD AI Assistant Early Access Secure Site](https://account.amd.com/en/member/vivado-ai-assistant-ea.html) and get an approval 
- Visual Studio Code + Github Copilot installed 
- Vivado 2025.2 installed
- Creating an account on GitHub (option for new user)
- Download related packages (Vivado AI Assistant Extension & Example Designs) from  [AMD AI Assistant Early Access Secure Site](https://account.amd.com/en/member/vivado-ai-assistant-ea.html)
![alt text](image.png) 

## Step 1 :  Install the Vivado AI Assistant Extension
- Download vivado-ai-extension-0.6.8.zip from the [Downloads](https://account.amd.com/en/member/vivado-ai-assistant-ea/getting-started/downloads.html) page and unzip it
- Open VS Code
- Go to Extensions sidebar → click ⋯ → Install from VSIX...
- Select the downloaded .vsix file
![alt text](image-1.png)
![alt text](image-2.png)

## Step 2 : Configure Vivado Path (Vivado AI Extension & system environment)
After installing the extension, set the path to your Vivado executable:
- Open Settings (Ctrl+,)
- Search for Vivado Path
- Enter the full path to your Vivado binary (e.g.,C:\AMD\DesignTools\2025.2\Vivado\bin\vivado.bat )
- To set the Vivado environment variable PATH, add the Vivado bin directory (such as C:\Xilinx\Vivado\<version>\bin) to your system environment variables.

![alt text](image-3.png)
![alt text](image-4.png)

## Step 3 :  Setup and Enable MCP Server
- In Github Copilt Chat -> Configure Tools...
- Enable Vivado-mcp-server checkbox

![alt text](image-5.png)

## Step 4 :  Verify the Setup
- login Github Copilot
- In Github Copilot Chat -> prompt 
- In Github Copilot Chat, Type: "List the available MCP tools"
- In Github Copilot Chat, Type: "Start a Vivado session"
- In Github Copilot Chat, Type: "How to configure NoC for optimal bandwidth? please first use vivado_doc_search tool"

![alt text](image-7.png)
![alt text](image-6.png)

## Step 5 (option) :  Install the Claude Code Extension
- VS Code -> Extension -> Claude Code for VS Code
- Install
- Ctrl + Shift + p -> Developer: Reload Window
 
 ![alt text](image-8.png)

## Step 6 (option) :  Setting MCP Server for Claude code
- create a "mcp.json" in workspace
- edit mcp.json to enable 

![alt text](image-9.png)

## Step 7 (option) : Verify the Setup for Claude Code
- login Claude Code
- In Claude Code Chat -> prompt 
- In Claude Code Chat, Type: "List the available MCP tools"
- In Claude Code Chat, Type: "How to configure NoC for optimal bandwidth?"

![alt text](image-10.png)