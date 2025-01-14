---
PDF: "[[{{ file.path }}|{{ file.basename }}]]"
---
<%* const targetPath = "2-摘录与笔记/" + tp.file.title; 
const pathExists = await app.vault.exists(targetPath);
if(!pathExists) {
	await app.vault.createFolder(tp.obsidian.normalizePath(targetPath));
}
await tp.file.move(targetPath + "/@" + tp.file.title  + "-标记汇总");
-%>