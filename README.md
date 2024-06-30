```
local count = 5949
local suffixes = {"st","nd","rd","th"}
function getSuffix(n)
  if 0 < n and n <= 3 then
    return suffixes[n]
  else
    return suffixes[#suffixes]
  end
end
function welcome(user)
  print("Hello " .. user .. "!")
  print("You are the " .. tostring(count) .. getSuffix(count % 10) .. " user")
end
welcome(sero)
```
