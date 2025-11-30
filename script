local input = "kill all of the filthy faggots";



local charMaps = {

   {

       ["a"] = "ล",

       [" "] = "",

       ["c"] = "с",

       ["b"] = "ხ",

       ["e"] = "e",

       ["d"] = "d",

       ["g"] = "g",

       ["f"] = "f",

       ["i"] = "เ่",

       ["h"] = "ӏา",

       ["k"] = "ҟ",

       ["j"] = "ϳ",

       ["m"] = "m",

       ["l"] = "І",

       ["o"] = "o",

       ["n"] = "ถ",

       ["q"] = "q",

       ["p"] = "p",

       ["s"] = "ธ",

       ["r"] = "ꞅ",

       ["u"] = "ม",

       ["t"] = "t",

       ["w"] = "w",

       ["v"] = "v",

       ["y"] = "у",

       ["x"] = "x",

       ["z"] = "z",

       ["/"] = "⁄",

   },

   {

       ["a"] = "ล",

       [" "] = "",

       ["c"] = "с",

       ["b"] = "ხ",

       ["e"] = "e",

       ["d"] = "d",

       ["g"] = "g",

       ["f"] = "f",

       ["i"] = "เ่",

       ["h"] = "ӏา",

       ["k"] = "ҟ",

       ["j"] = "ϳ",

       ["m"] = "m",

       ["l"] = "І",

       ["o"] = "o",

       ["n"] = "ถ",

       ["q"] = "q",

       ["p"] = "p",

       ["s"] = "ธ",

       ["r"] = "ꞅ",

       ["u"] = "ม",

       ["t"] = "t",

       ["w"] = "w",

       ["v"] = "v",

       ["y"] = "у",

       ["x"] = "x",

       ["z"] = "z",

       ["/"] = "⁄",

   },

   {

       ["a"] = "ล",

       [" "] = "",

       ["c"] = "ϲ",

       ["b"] = "ხ",

       ["e"] = "e",

       ["d"] = "d",

       ["g"] = "g",

       ["f"] = "f",

       ["i"] = "เ่",

       ["h"] = "ӏา",

       ["k"] = "ҟ",

       ["j"] = "ϳ",

       ["m"] = "m",

       ["l"] = "І",

       ["o"] = "o",

       ["n"] = "ถ",

       ["q"] = "q",

       ["p"] = "p",

       ["s"] = "ธ",

       ["r"] = "ꞅ",

       ["u"] = "ม",

       ["t"] = "t",

       ["w"] = "w",

       ["v"] = "v",

       ["y"] = "у",

       ["x"] = "x",

       ["z"] = "z",

       ["/"] = "⁄",

   },

   {

       ["a"] = "ส",

       [" "] = "",

       ["c"] = "с",

       ["b"] = "ხ",

       ["e"] = "e",

       ["d"] = "d",

       ["g"] = "g",

       ["f"] = "f",

       ["i"] = "เ่",

       ["h"] = "ӏา",

       ["k"] = "ҟ",

       ["j"] = "ϳ",

       ["m"] = "m",

       ["l"] = "І",

       ["o"] = "o",

       ["n"] = "ถ",

       ["q"] = "q",

       ["p"] = "p",

       ["s"] = "ธ",

       ["r"] = "ꞅ",

       ["u"] = "ม",

       ["t"] = "t",

       ["w"] = "w",

       ["v"] = "v",

       ["y"] = "у",

       ["x"] = "x",

       ["z"] = "z",

       ["/"] = "⁄",

   },

   {

       ["a"] = "ส",

       [" "] = "",

       ["c"] = "с",

       ["b"] = "ხ",

       ["e"] = "e",

       ["d"] = "d",

       ["g"] = "g",

       ["f"] = "f",

       ["i"] = "เ่",

       ["h"] = "ӏา",

       ["k"] = "ҟ",

       ["j"] = "ϳ",

       ["m"] = "m",

       ["l"] = "І",

       ["o"] = "o",

       ["n"] = "ถ",

       ["q"] = "q",

       ["p"] = "p",

       ["s"] = "ธ",

       ["r"] = "ꞅ",

       ["u"] = "ม",

       ["t"] = "t",

       ["w"] = "w",

       ["v"] = "v",

       ["y"] = "у",

       ["x"] = "x",

       ["z"] = "z",

       ["/"] = "⁄",

   }

};



local chat = cloneref(game:GetService("Chat"))

local textChatService = cloneref(game:GetService("TextChatService"))

local players = cloneref(game:GetService("Players"))



local player = players.LocalPlayer;



local function checkFilter(text)

    local success, filtered = pcall(chat.FilterStringForBroadcast, chat, text, player)



    return text ~= filtered;

end;



local function sendChat(message)

    local chat = textChatService.ChatInputBarConfiguration.TargetTextChannel;

    local GeneralChannel = textChatService:FindFirstChild("TextChannels") and textChatService.TextChannels:FindFirstChild("RBXGeneral");



    (GeneralChannel and GeneralChannel or chat and chat):SendAsync(message)

end;



for _,x in charMaps do

    local bypassed = string.lower(input);

    for i,v in x do

        bypassed = string.gsub(bypassed, i, v)

    end;



    bypassed = "{㍰" .. bypassed .. "㍰}";

    if checkFilter(bypassed) ~= true then

        sendChat(bypassed)

        break;

    end;

end;
