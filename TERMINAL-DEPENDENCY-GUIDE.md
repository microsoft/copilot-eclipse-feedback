# Resolving Terminal Dependency Issues in Copilot for Eclipse

When using the Copilot plugin in Eclipse, Copilot requires the IDE to have terminal-related dependencies installed in order to support the `runInTerminal` tool in Agent Mode.

If these dependencies are missing, Copilot will still function normally for most features, but `runInTerminal` cannot execute properly. When the IDE starts, you will see a dialog notifying you about the missing terminal dependencies. 
<img width="1045" height="634" alt="image" src="https://github.com/user-attachments/assets/045708aa-51d8-40d8-953b-4474c5026973" />

If you do not plan to use the `runInTerminal` tool, you may choose **"Don't show this message again"**, and this will not affect any other Copilot features.

This guide explains how to install the required terminal features to fully enable `runInTerminal` support.

## Steps to Fix the Terminal Dependency Issue

### 1. Open the "Install New Software" Dialog

In Eclipse, click **Help → Install New Software…**
<img width="3839" height="2091" alt="图像 (1)" src="https://github.com/user-attachments/assets/61e9ca5a-fe00-40e3-ad68-83fd77b6afee" />


### 2. Select All Available Sites

In the Install dialog, find the **Work with** dropdown and select **All Available Sites**.
<img width="1970" height="1063" alt="图像 (2)" src="https://github.com/user-attachments/assets/2916fdcf-9d9f-4fc4-8b55-461c246ecc87" />


### 3. Search for the Required Terminal Feature

Use the search box to look for the correct terminal feature based on your IDE version:

| Eclipse IDE Version | Feature Name to Search |
|---------------------|------------------------|
| Before 2025-09 | TM Terminal |
| 2025-09 and later | Terminal Feature |

**Before 2025-09**

<img width="1970" height="1065" alt="图像 (3)" src="https://github.com/user-attachments/assets/b3ebca28-99ef-4869-be16-3f5c3b2662b6" />

**2025-09 and later**

<img width="1968" height="1066" alt="图像 (4)" src="https://github.com/user-attachments/assets/fe4b4c57-0555-4174-a971-c05310317762" />


### 4. Locate and Install the Matching Feature

1. Wait for the search results to load (this may take some time)
2. Expand the result categories
3. Select the correct terminal feature
4. Click **Next** to download and install

**Before 2025-09**

<img width="1973" height="1068" alt="图像 (6)" src="https://github.com/user-attachments/assets/333aab23-09c0-4a13-9fae-83d4879de479" />

**2025-09 and later**

<img width="1968" height="1061" alt="图像 (5)" src="https://github.com/user-attachments/assets/9f1db515-570a-4cf7-b23f-dde726e83689" />



### 5. Restart the IDE

After installation completes, Eclipse will prompt you to restart.

Once restarted, Copilot will work with full terminal support, and the `runInTerminal` tool will function normally.
