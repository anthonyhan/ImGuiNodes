# ImGuiNodes

a fork of the gist from https://gist.github.com/ChemistAion/0cd64b71711d81661344af040c142c1c

original author: [ChemistAion](https://github.com/ChemistAion)

this repository is created for better version control and generation of its [c-api wrapper](https://github.com/anthonyhan/cimgui_nodes).

## Usage
```
static ImGui::ImGuiNodes nodes_;
//...
ImGui::Begin("Nodes II");
nodes_.Update();
nodes_.ProcessNodes();
nodes_.ProcessContextMenu();
ImGui::End();
//...
```
## Legend

Mouse left-button: selection (shift/ctrl modifiers), node dragging, making new connections;

Mouse left-button double click: node collapsing, reassign input (delete previous one);

Mouse right-button: new nodes (pop-up), canvas movement;

Mouse right-button double click: toggling node as disabled;

Mouse wheel-button: canvas movement/zooming (shift/ctrl modifiers);

Delete-key: deletes all currently selected nodes

*Ref: https://github.com/ocornut/imgui/issues/306#issuecomment-1017918768*
