This repo presently contains my modifications to existing plugins.

<img width="1226" height="772" alt="image" src="https://github.com/user-attachments/assets/8bbb6515-437f-4e57-b44b-60730ecadd2e" />

Changes shown:
1. Updated `RnameWithGMCP` to display room area keyword as a clickable link in addition to room id.
2. Updated `HyperlinkMapperNotes` to uses backticks to embedded commands in mapper notes.
3. Updated `HyperlinkMapperNotes` to display parsed commands below room exits.
4. Updated `HyperlinkMapperNotes` to allow the `mappernotecommand` to be called with an index so all configured commands can be executed without resorting to clicking.

Changes not shown:
1. Updated `Aardwolf_Rich_Exits` to fix a bug where it wouldnt show a custom exit that matches a cardinal direction when the cardinal direction exit had a missing vnum (hidden exit). It now using the exit vnum of the custom exit.
2. Updated `Aardwolf_Rich_Exits`  to modify the `cexit` alias to allow for `n` `e` `s` `w` `u` `d` in addition to the numerical cexit index. This means I can bind cexit (neswud) to my numpad direction keys and it will handle door cexits automatically if present.
3. Updated `GQ_List` to fix a bug where the plugin would error when no Global Quests were active due to `row_del` being nil. (Same fix as this: https://github.com/Memnoch1244/GQ-List/pull/2)
