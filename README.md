- 👋 Hi, I’m @learningHowCode
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
learningHowCode/learningHowCode is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
------>
FormatTable({a, "b", 1, game:GetService("Players"), pcall})

FormatTable({ workspace, 20, { pcall, 0X20 } }, {
    OneLine = true;
    IgnoreNumberIndex = true;
    NoIndentation = false;
    MetatableKey = nil;
    GenerateScript = false;
    NoAntiRep = false;
    LargeStrings = false;
})

FormatArguments(a, "b", 1, game:GetService("Players"), pcall)

local Result = FormatTable({ 1, "b", game:GetService("Players").LocalPlayer}, {
    OneLine = false;
    IgnoreNumberIndex = false;
    NoIndentation = false;
    MetatableKey = Key;
    GenerateScript = true;
    NoAntiRep = false;
    LargeStrings = false;
}) --// Will return a table with two arguments, [1] will contain FindFunction(), [2] will contain the generated code

local Proxy, Key = newproxy(true), game:GetService("HttpService"):GenerateGUID(false)
setrawmetatable(Proxy, {
    [Key] = "Hello there"
})
FormatTable({ workspace, 20, Proxy }, {
    OneLine = false;
    IgnoreNumberIndex = false;
    NoIndentation = false;
    MetatableKey = Key;
    GenerateScript = false;
    NoAntiRep = false;
    LargeStrings = false;
})

