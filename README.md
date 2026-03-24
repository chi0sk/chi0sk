<div align="center">
  <img src="banner.png" alt="sam / @chi0sk banner" width="100%">

  <h3>hey, i'm sam (@chi0sk)</h3>
  <p>16. writing code mostly in luau and c++.</p>
</div>

---

<h3 align="center"><img src="https://api.iconify.design/lucide:mail.svg?color=%23888888" width="20" align="center" alt="contact" /> contact</h3>

<div align="center">
  <b>discord:</b> <code>rituals._</code><br>
  <b>roblox:</b> <a href="https://www.roblox.com/users/profile?username=chi0sk">chi0sk</a>
</div>

---

<h3 align="center"><img src="https://api.iconify.design/lucide:terminal.svg?color=%23888888" width="20" align="center" alt="tech" /> tech</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Luau-00A2FF?style=for-the-badge&logo=lua&logoColor=white" alt="Luau" />
  <img src="https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white" alt="C++" />
  <img src="https://img.shields.io/badge/Roblox_Studio-000000?style=for-the-badge&logo=roblox&logoColor=white" alt="Roblox Studio" />
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" alt="Git" />
</p>

---

<h3 align="center"><img src="https://api.iconify.design/lucide:cog.svg?color=%23888888" width="20" align="center" alt="building" /> currently building</h3>

<div align="center">

#### [sift](https://github.com/chi0sk/sift)
a luau bytecode decompiler that focuses on producing code you can actually read.

it takes compiled luau bytecode and reconstructs it into something close to the original source, instead of dumping low-level instructions or unreadable output.

<br>

<details>
<summary><b>view decompilation example</b></summary>
<div align="left">

<br>

**original source:**

```lua
local a = true
if a then print("yes") else print("no") end
for i = 1, 10 do print(i) end
function outer() return function() print("inner") end end
local x = 10
function test() print(x) end
local t = {a = 1, b = 2}
print(t.a)
function f(...) print(...) end
```
**original source was then compiled and inputted into sift --->**

**sift output:**

```lua
if true then
	print("yes")
else
	print("no")
end
for i = 1, 10 do
	print(i)
end
function outer()
	return function()
		print("inner")
	end
end
function test()
	print(x)
end
local t = { a = 1, b = 2 }
print(t.a)
function f(...)
	print(...)
end
```
