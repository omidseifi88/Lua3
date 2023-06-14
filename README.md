DateE = "2024/06/07 15:00:00PM"
DateToday = os.date("%Y/%m/%d %H:%M:%S%p")
if DateToday >= DateE then
gg.alert("مهلت استفاده از چیت به پایان رسیده است.")
gg.alert("♥︎★【PM:@KING_IRAN_DEAR】★♥︎\n♥︎★【PM:@AFGHANBAD】★♥︎\n♥︎★【CHANNEL:@XCHEATCODM】★♥︎")
print("KING🤴IRAN")
print("@XCHEATCODM\nبرای دریافت اسکریپت جدید به چنل تلگرامی ما مراجعه نمایید.👆👆🔵🔴🟢")
os.exit()
return
end


--[[pass = gg.prompt({"USERNAME","PASSWORD","LOGO BYPASS","FIX CRASH"},nil, {"","","checkbox","checkbox"})
if pass[1] == "omid" and pass[2] == "seifi" then
gg.alert("LOGIN ACCOUNT✅️")
else
gg.alert("LOGIN ACCOUNT❌️⚠️")
print("BUY ACCOUNT📱:\nt.me/KING_IRAN02")
return
end
if pass[3] and pass[4] == "or" or "1" then
gg.setRanges(gg.REGION_C_DATA)
gg.searchNumber("1,159,943,203;1,394,823,715;1,193,494,819;1,096,045,347;1,684,524,592;1000000000~2000000000::16384", gg.TYPE_DWORD, false, gg.SIGN_EQUAL, 0, -1)
revert = gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil)
local t = gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil)
for i, v in ipairs(t) do
if v.flags == gg.TYPE_DWORD then
v.value = "0"
v.freeze = true
end
end
gg.addListItems(t)
t = nil
function setvalue(address,flags,value)
 local tt={} tt[1]={} tt[1].address=address tt[1].flags=flags tt[1].value=value gg.setValues(tt) end
so=gg.getRangesList('libanogs.so')[1].start
py=0x718A8
setvalue(so+py,4,0)
gg.toast("فیکس کرش با موفقیت فعال شد.✅️")
gg.clearList()
gg.clearResults()
gg.processResume()
end]]


function patch(lib, offset, value, flags)
  local ranges = gg.getRangesList(lib)
  if #ranges == 0 then
    gg.toast("Error: " .. lib .. " not found")
  else
    local a = {}
    a[1] = {}
    a[1].address = ranges[1].start + offset
    a[1].flags = flags
    a[1].value = value
    gg.setValues(a)
  end
end

function hexpatch(lib, offset, value, flags)
  local ranges = gg.getRangesList(lib)
  if #ranges == 0 then
    gg.toast("Error: " .. lib .. " not found")
  else
    local a = {}
    a[1] = {}
    a[1].address = ranges[1].start + offset
    a[1].flags = flags
    a[1].value = value .. "r"
    gg.setValues(a)
  end
end
function split(szFullString, szSeparator) local nFindStartIndex = 1 local nSplitIndex = 1 local nSplitArray = {} while true do local nFindLastIndex = string.find(szFullString, szSeparator, nFindStartIndex) if not nFindLastIndex then nSplitArray[nSplitIndex] = string.sub(szFullString, nFindStartIndex, string.len(szFullString)) break end nSplitArray[nSplitIndex] = string.sub(szFullString, nFindStartIndex, nFindLastIndex - 1) nFindStartIndex = nFindLastIndex + string.len(szSeparator) nSplitIndex = nSplitIndex + 1 end return nSplitArray end function xgxc(szpy, qmxg) for x = 1, #(qmxg) do xgpy = szpy + qmxg[x]["offset"] xglx = qmxg[x]["type"] xgsz = qmxg[x]["value"] gg.setValues({[1] = {address = xgpy, flags = xglx, value = xgsz}}) xgsl = xgsl + 1 end end function xqmnb(qmnb) gg.clearResults() gg.setRanges(qmnb[1]["memory"]) gg.searchNumber(qmnb[3]["value"], qmnb[3]["type"]) if gg.getResultCount() == 0 then gg.toast(qmnb[2]["name"] ..
"开启失败") else gg.refineNumber(qmnb[3]["value"], qmnb[3]["type"]) gg.refineNumber(qmnb[3]["value"], qmnb[3]["type"]) gg.refineNumber(qmnb[3]["value"], qmnb[3]["type"]) if gg.getResultCount() == 0 then gg.toast(qmnb[2]["name"] .. "开启失败") else sl = gg.getResults(999999) sz = gg.getResultCount() xgsl = 0 if sz > 999999 then sz = 999999 end for i = 1, sz do pdsz = true for v = 4, #(qmnb) do if pdsz == true then pysz = {} pysz[1] = {} pysz[1].address = sl[i].address + qmnb[v]["offset"] pysz[1].flags = qmnb[v]["type"] szpy = gg.getValues(pysz) pdpd = qmnb[v]["lv"] .. ";" .. szpy[1].value szpd = split(pdpd, ";") tzszpd = szpd[1] pyszpd = szpd[2] if tzszpd == pyszpd then pdjg = true pdsz = true else pdjg = false pdsz = false end end end if pdjg == true then szpy = sl[i].address xgxc(szpy, qmxg) xgjg = true end end if xgjg == true then gg.toast(qmnb[2]["name"] .. "开启成功,共修改" .. xgsl .. "条数据") else gg.toast(qmnb[2]["name"] .. "开启失败") end end end end
function split(szFullString, szSeparator) local nFindStartIndex = 1 local nSplitIndex = 1 local nSplitArray = {} while true do local nFindLastIndex = string.find(szFullString, szSeparator, nFindStartIndex) if not nFindLastIndex then nSplitArray[nSplitIndex] = string.sub(szFullString, nFindStartIndex, string.len(szFullString)) break end nSplitArray[nSplitIndex] = string.sub(szFullString, nFindStartIndex, nFindLastIndex - 1) nFindStartIndex = nFindLastIndex + string.len(szSeparator) nSplitIndex = nSplitIndex + 1 end return nSplitArray end function xgxc(szpy, Loading1) for x = 1, #(Loading1) do xgpy = szpy + Loading1[x]["address"] xglx = Loading1[x]["flags"] xgsz = Loading1[x]["value"] xgdj = Loading1[x]["freeze"] if xgdj == nil or xgdj == "" then gg.setValues({[1] = {address = xgpy, flags = xglx, value = xgsz}}) else gg.addListItems({[1] = {address = xgpy, flags = xglx, freeze = xgdj, value = xgsz}}) end xgsl = xgsl + 1 xgjg = true end end function LoadingQ(Loading) gg.setRanges(Loading[1]["memory"]) gg.searchNumber(Loading[3]["value"], Loading[3]["flags"]) if gg.getResultCount() == 0 then gg.toast(Loading[2]["Projects"] .. "Load失败❌") else gg.refineNumber(Loading[3]["value"], Loading[3]["flags"]) gg.refineNumber(Loading[3]["value"], Loading[3]["flags"]) gg.refineNumber(Loading[3]["value"], Loading[3]["flags"]) if gg.getResultCount() == 0 then gg.toast(Loading[2]["Projects"] .. "Load失败❌") else sl = gg.getResults(999999) sz = gg.getResultCount() xgsl = 0 if sz > 999999 then sz = 999999 end for i = 1, sz do pdsz = true for v = 4, #(Loading) do if pdsz == true then pysz = {} pysz[1] = {} pysz[1].address = sl[i].address + Loading[v]["address"] pysz[1].flags = Loading[v]["flags"] szpy = gg.getValues(pysz) pdpd = Loading[v]["lv"] .. ";" .. szpy[1].value szpd = split(pdpd, ";") tzszpd = szpd[1] pyszpd = szpd[2] if tzszpd == pyszpd then pdjg = true pdsz = true else pdjg = false pdsz = false end end end if pdjg == true then szpy = sl[i].address xgxc(szpy, Loading1) end end if xgjg == true then 
end end end end
function edit(orig,ret)_om=orig[1].memory or orig[1][1]_ov=orig[3].value or orig[3][1]_on=orig[2].name or orig[2][1]
gg.clearResults()gg.setRanges(_om)gg.searchNumber(_ov,orig[3].type or orig[3][2])sz=gg.getResultCount()if sz<1 then gg.toast(_on.." 开启失败")else sl=gg.getResults(50000)for a=1,sz do ist=true for v=4,#orig do if ist==true and sl[i].value==_ov then cd={{}}cd[1].address=sl[i].address+(orig[v].offset or orig[v][2])cd[1].flags=orig[v].type or orig[v][3]szpy=gg.getValues(cd)cdlv=orig[v].lv or orig[v][1]cdv=szpy[1].value if cdlv==cdv then pdjg=true ist=true else pdjg=false ist=false end end end if pdjg==true then szpy=sl[i].address for x=1,#(ret)do xgpy=szpy+(ret[x].offset or ret[x][2])xglx=ret[x].type or ret[x][3]xgsz=ret[x].value or ret[x][1]xgdj=ret[x].freeze or ret[x][4]xgsj={{address=xgpy,flags=xglx,value=xgsz}}if xgdj==true then xgsj[1].freeze=xgdj gg.addListItems(xgsj)else gg.setValues(xgsj)end end xgjg=true end end if xgjg==true then gg.toast(_on.." 开启成功")else gg.toast(_on.." 开启失败")end end end
local app = {}
app.memorySearchMode = function(MEMORY) 
if (MEMORY == 2) then
gg.setRanges(gg.REGION_JAVA_HEAP | gg.REGION_C_HEAP | gg.REGION_C_ALLOC | gg.REGION_C_DATA | gg.REGION_C_BSS | gg.REGION_PPSSPP) 
end 
if (MEMORY == -1) then
gg.setRanges(gg.REGION_VIDEO) 
end 
if (MEMORY == -2) then 
gg.setRanges(gg.REGION_CODE_APP | gg.REGION_CODE_SYS)         
end 
if (MEMORY == 0) then 
gg.setRanges(gg.REGION_ANONYMOUS)
end        
end
function checkType(dataType) local type 
if dataType =="D" or dataType == "D" then 
type = gg.TYPE_DWORD 
end 
if dataType == "F" then 
type = gg.TYPE_FLOAT 
end 
if dataType == "E" then 
type = gg.TYPE_DOUBLE 
end 
if dataType == "B" or dataType == "B" then 
type =  gg.TYPE_BYTE 
end 
if dataType == "W" or dataType == "W" then 
type = gg.TYPE_WORD os.exit() 
end 
return type 
end
app.memorySearch = function(pkgName, isNewSearch, address, tb, dataType) 
gg.clearResults() 
gg.setVisible(false) local isSucess = gg.searchNumber(tb[1]["lv"], checkType(dataType), false, gg.SIGN_EQUAL, address, -1); local t = gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil); local tab = {} local data = {} for a=1, #t do for j=2, #tb do tab[j] = {} tab[j].address = t[i].address + tb[j]["offset"] if(tb[j]["type"] == nil) then tab[j].flags = t[i].flags else tab[j].flags = checkType(tb[j]["type"]) end tab = gg.getValues(tab) if (tab[j].value == tb[j]["lv"]) then data[#data+1] = t[i].address end end end gg.clearResults() return isSucess, data end app.memoryWrite = function(pkgName, address, value, dataType) gg.setVisible(false) local t = {} t[1] ={} t[1].address = address t[1].flags = checkType(dataType) t[1].value = value return gg.setValues(t) end
GG = {Read,Write} 
function GG.ReadWrite(Read,Writw)TZ = {} dataTZ = Read[1] offset = dataTZ[2] for a=1,#Read do TZA = Read[i] LV = {["lv"] = TZA[1],["offset"] = TZA[2]-offset} table.insert(TZ, i, LV) end app.memorySearchMode(Memory) isSuuess,TUG = app.memorySearch(pkgName, true, 0, TZ, Type) if TUG[1] == nil then  else for ia=1,#TUG do for iia=1,#Write do dataxg = Write[iii] value = dataxg[1] Deviant = dataxg[2] app.memoryWrite(pkgName,TUG[ii]+Deviant-offset,value,Type) end end gg.toast(ID.. "开启成功") end end
function SearchWrite(Search, Write, Type)
gg.clearResults()
gg.setVisible(false)
gg.searchNumber(Search[1][1], Type)
local t = gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.clearResults()
if t ~= nil then
local r = {}
for j=2, #Search do
for i, v in ipairs(t) do
r[i] = {}
r[i].address = v.address + Search[j][2] - Search[1][2]
r[i].flags = v.flags
end
r = gg.getValues(r)
for i = #t, 1, -1 do
if (tostring(r[i].value) ~= tostring(Search[j][1]) ) then
table.remove(t, i)
table.remove(r, i)
end
end       
end
--写入数据
local r = {}
for a=1, #t do
for j=1, #Write do
r[#r+1] = {}
r[#r].address = t[i].address + Write[j][2] - Search[1][2]
r[#r].flags = t[i].flags
r[#r].value = Write[j][1]
r[#r].freeze = true--冻结的话修改后面加false
end
end
gg.setValues(r)
end
end
--gg.addListItems(r)
function split(szFullString, szSeparator) local nFindStartIndex = 1 local nSplitIndex = 1 local nSplitArray = {} while true do local nFindLastIndex = string.find(szFullString, szSeparator, nFindStartIndex) if not nFindLastIndex then nSplitArray[nSplitIndex] = string.sub(szFullString, nFindStartIndex, string.len(szFullString)) break end nSplitArray[nSplitIndex] = string.sub(szFullString, nFindStartIndex, nFindLastIndex - 1) nFindStartIndex = nFindLastIndex + string.len(szSeparator) nSplitIndex = nSplitIndex + 1 end return nSplitArray end function xgxc(szpy, qmxg) for x = 1, #(qmxg) do xgpy = szpy + qmxg[x]["offset"] xglx = qmxg[x]["type"] xgsz = qmxg[x]["value"] gg.setValues({[1] = {address = xgpy, flags = xglx, value = xgsz}}) xgsl = xgsl + 1 end end function xqmnb(qmnb) gg.clearResults() gg.setRanges(qmnb[1]["memory"]) gg.searchNumber(qmnb[3]["value"], qmnb[3]["type"]) if gg.getResultCount() == 0 then gg.toast(qmnb[2]["name"] .. "开启失败") else gg.refineNumber(qmnb[3]["value"], qmnb[3]["type"]) gg.refineNumber(qmnb[3]["value"], qmnb[3]["type"]) gg.refineNumber(qmnb[3]["value"], qmnb[3]["type"]) if gg.getResultCount() == 0 then gg.toast(qmnb[2]["name"] ..
"开启失败") else sl = gg.getResults(999999) sz = gg.getResultCount() xgsl = 0 if sz > 999999 then sz = 999999 end for i = 1, sz do pdsz = true for v = 4, #(qmnb) do if pdsz == true then pysz = {} pysz[1] = {} pysz[1].address = sl[i].address + qmnb[v]["offset"] pysz[1].flags = qmnb[v]["type"] szpy = gg.getValues(pysz) pdpd = qmnb[v]["lv"] .. ";" .. szpy[1].value szpd = split(pdpd, ";") tzszpd = szpd[1] pyszpd = szpd[2] if tzszpd == pyszpd then pdjg = true pdsz = true else pdjg = false pdsz = false end end end if pdjg == true then szpy = sl[i].address xgxc(szpy, qmxg) xgjg = true end end if xgjg == true then gg.toast(qmnb[2]["name"] .. "开启成功,共修改" .. xgsl .. "条数据") else gg.toast(qmnb[2]["name"] .. "开启失败") end end end end
function SearchWrite(Search, Write, Type)
gg.clearResults()
gg.setVisible(false)
gg.searchNumber(Search[1][1], Type)
local count = gg.getResultCount()
local result = gg.getResults(count)
gg.clearResults()
local data = {}
local base = Search[1][2] 
if (count > 0) then
for i, v in ipairs(result) do
v.isUseful = true 
end
for k=2, #Search do
local MRp = {}
local offset = Search[k][2] - base 
local num = Search[k][1] 
for i, v in ipairs(result) do
MRp[#MRp+1] = {} 
MRp[#MRp].address = v.address + offset  
MRp[#MRp].flags = v.flags  
end
MRp = gg.getValues(MRp) 
for i, v in ipairs(MRp) do
if ( tostring(v.value) ~= tostring(num) ) then 
result[i].isUseful = false 
end
end
end
for i, v in ipairs(result) do
if (v.isUseful) then 
data[#data+1] = v.address
end
end
if (#data > 0) then
gg.toast("搜索η"..#data.."条ΔΘ")
local t = {}
local base = Search[1][2]
for a=1, #data do
for k, w in ipairs(Write) do
offset = w[2] - base
t[#t+1] = {}
t[#t].address = data[i] + offset
t[#t].flags = Type
t[#t].value = w[1]
if (w[3] == true) then
local item = {}
item[#item+1] = t[#t]
item[#item].freeze = true
gg.addListItems(item)
end
end
end
gg.setValues(t)
else
gg.toast("not found", false)
return false
end
else
gg.toast("Not Found")
return false
end
end
function split(szFullString, szSeparator) local nFindStartIndex = 1 local nSplitIndex = 1 local nSplitArray = {} while true do local nFindLastIndex = string.find(szFullString, szSeparator, nFindStartIndex) if not nFindLastIndex then nSplitArray[nSplitIndex] = string.sub(szFullString, nFindStartIndex, string.len(szFullString)) break end nSplitArray[nSplitIndex] = string.sub(szFullString, nFindStartIndex, nFindLastIndex - 1) nFindStartIndex = nFindLastIndex + string.len(szSeparator) nSplitIndex = nSplitIndex + 1 end return nSplitArray end function xgxc(szpy, qmxg) for x = 1, #(qmxg) do xgpy = szpy + qmxg[x]["offset"] xglx = qmxg[x]["type"] xgsz = qmxg[x]["value"] xgdj = qmxg[x]["freeze"] if xgdj == nil or xgdj == "" then gg.setValues({[1] = {address = xgpy, flags = xglx, value = xgsz}}) else gg.addListItems({[1] = {address = xgpy, flags = xglx, freeze = xgdj, value = xgsz}}) end xgsl = xgsl + 1 xgjg = true end end function xqmnb(qmnb) gg.clearResults() gg.setVisible(false) gg.setRanges(qmnb[1]["memory"]) gg.searchNumber(qmnb[3]["value"], qmnb[3]["type"]) if gg.getResultCount() == 0 then gg.toast(qmnb[2]["name"] .. " Failed") else gg.refineNumber(qmnb[3]["value"], qmnb[3]["type"]) gg.refineNumber(qmnb[3]["value"], qmnb[3]["type"]) gg.refineNumber(qmnb[3]["value"], qmnb[3]["type"]) fff=gg.getResultCount() if gg.getResultCount() == 0 then gg.toast(qmnb[2]["name"] .. " Failed") else sl = gg.getResults(999999) sz = gg.getResultCount() xgsl = 0 if sz > 999999 then sz = 999999 end for i = 1, sz do pdsz = true for v = 4, #(qmnb) do if pdsz == true then pysz = {} pysz[1] = {} pysz[1].address = sl[i].address + qmnb[v]["offset"] pysz[1].flags = qmnb[v]["type"] szpy = gg.getValues(pysz) pdpd = qmnb[v]["lv"] .. ";" .. szpy[1].value szpd = split(pdpd, ";") tzszpd = szpd[1] pyszpd = szpd[2] if tzszpd == pyszpd then pdjg = true pdsz = true else pdjg = false pdsz = false end end end if pdjg == true then szpy = sl[i].address xgxc(szpy, qmxg) end end if xgjg == true then gg.toast(qmnb[2]["name"] .. "\nFound: "..fff.." Edited: " .. xgsl .. "") else gg.toast(qmnb[2]["name"] .. " Failed") end end end gg.clearResults()  end
function PS() end
function setvalue(address,flags,value) local tt={} tt[1]={} tt[1].address=address tt[1].flags=flags tt[1].value=value gg.setValues(tt) end

function split(szFullString, szSeparator) local nFindStartIndex = 1 local nSplitIndex = 1 local nSplitArray = {} while true do local nFindLastIndex = string.find(szFullString, szSeparator, nFindStartIndex) if not nFindLastIndex then nSplitArray[nSplitIndex] = string.sub(szFullString, nFindStartIndex, string.len(szFullString)) break end nSplitArray[nSplitIndex] = string.sub(szFullString, nFindStartIndex, nFindLastIndex - 1) nFindStartIndex = nFindLastIndex + string.len(szSeparator) nSplitIndex = nSplitIndex + 1 end return nSplitArray end function xgxc(szpy, qmxg) for x = 1, #(qmxg) do xgpy = szpy + qmxg[x]["offset"] xglx = qmxg[x]["type"] xgsz = qmxg[x]["value"] xgdj = qmxg[x]["freeze"] if xgdj == nil or xgdj == "" then gg.setValues({[1] = {address = xgpy, flags = xglx, value = xgsz}}) else gg.addListItems({[1] = {address = xgpy, flags = xglx, freeze = xgdj, value = xgsz}}) end xgsl = xgsl + 1 xgjg = true end end function xqmnb(qmnb) gg.clearResults() gg.setVisible(false) gg.setRanges(qmnb[1]["memory"]) gg.searchNumber(qmnb[3]["value"], qmnb[3]["type"]) if gg.getResultCount() == 0 then gg.toast(qmnb[2]["name"] .. " Failed") else gg.refineNumber(qmnb[3]["value"], qmnb[3]["type"]) gg.refineNumber(qmnb[3]["value"], qmnb[3]["type"]) gg.refineNumber(qmnb[3]["value"], qmnb[3]["type"]) sss=gg.getResultCount() if gg.getResultCount() == 0 then gg.toast(qmnb[2]["name"] .. " Failed") else sl = gg.getResults(999999) sz = gg.getResultCount() xgsl = 0 if sz > 999999 then sz = 999999 end for i = 1, sz do pdsz = true for v = 4, #(qmnb) do if pdsz == true then pysz = {} pysz[1] = {} pysz[1].address = sl[i].address + qmnb[v]["offset"] pysz[1].flags = qmnb[v]["type"] szpy = gg.getValues(pysz) pdpd = qmnb[v]["lv"] .. ";" .. szpy[1].value szpd = split(pdpd, ";") tzszpd = szpd[1] pyszpd = szpd[2] if tzszpd == pyszpd then pdjg = true pdsz = true else pdjg = false pdsz = false end end end if pdjg == true then szpy = sl[i].address xgxc(szpy, qmxg) end end if xgjg == true then gg.toast(qmnb[2]["name"] .. "\nFound: "..sss.." Edited: " .. xgsl .. "") else gg.toast(qmnb[2]["name"] .. " Failed") end end end gg.clearResults()  end
function PS() end
function setvalue(address,flags,value) local tt={} tt[1]={} tt[1].address=address tt[1].flags=flags tt[1].value=value gg.setValues(tt) end
function patch(lib, offset, value, flags)
local ranges = gg.getRangesList(lib)
if #ranges == 0 then
gg.toast("Error: " .. lib .. " not found")
else
local a = {}
a[1] = {}
a[1].address = ranges[1].start + offset
a[1].flags = flags
a[1].value = value
gg.setValues(a)
end
end

MenU = 1
function home()
MenUU = gg.choice({
"منوی بای پس",
"منوی لابی",
"منوی گیم",
"خروج",
}, nil, os.date("%A %d %B %T %Y/%m/%d"))
if MenUU == nil then end
if MenUU == 1 then 
bypass() end

if MenUU == 2 then 
labychits() end

if MenUU == 3 then 
gamechits() end

if MenUU == 4 then 
EXIT1() end

MenU =-1
end

function bypass()
OMIDSEIFI = gg.multiChoice({
"بای پس لوگو",
"فیکس کرش",
"بای پس لابی",
"ریپورت بلاک گر",
"آنتی چکر",
"چکر آنتی بن",
"برگشت",
}, nil, os.date("%A %d %B %T %Y/%m/%d"))
if OMIDSEIFI == nil then else
if OMIDSEIFI [1] == true then bylogo() end
if OMIDSEIFI [2] == true then byfix() end
if OMIDSEIFI [3] == true then byloby() end
if OMIDSEIFI [4] == true then report() end
if OMIDSEIFI [5] == true then anti() end
if OMIDSEIFI [6] == true then antibancheker() end
if OMIDSEIFI [7] == true then home() end
end
OMIDSEIFI = 1
end

function bylogo()
gg.setRanges(gg.REGION_C_DATA)
gg.searchNumber("1,159,943,203;1,394,823,715;1,193,494,819;1,096,045,347;1,684,524,592;1000000000~2000000000", gg.TYPE_DWORD, false, gg.SIGN_EQUAL, 0, -1)
revert = gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil)
local t = gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil)
for i, v in ipairs(t) do
if v.flags == gg.TYPE_DWORD then
v.value = "0"
v.freeze = true
end
end
gg.addListItems(t)
t = nil
gg.clearResults()
gg.clearList()
gg.alert("لوگو بای پس با موفقیت فعال شد.✅")
end

function byfix()
so = gg.getRangesList('libanogs.so')[1].start
py = 0x718A8
setvalue(so + py, 4, 0)
gg.alert("فیکس کرش با موفقیت فعال شد.✅️")
end


function byloby()
gg.setRanges(gg.REGION_CODE_APP)
gg.searchNumber("1,179,403,647;1,685,382,481;1,879,048,193;1,685,382,482;1,919,184,449;1000000000~2000000000::16384", gg.TYPE_DWORD, false, gg.SIGN_EQUAL, 0, -1)
revert = gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil)
local t = gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil)
for i, v in ipairs(t) do
if v.flags == gg.TYPE_DWORD then
v.value = "0"
v.freeze = true
end
end
gg.addListItems(t)
t = nil
gg.clearResults()
gg.clearList()
gg.alert("لابی بای پس با موفقیت فعال شد.✅")
end

function anti()
gg.setRanges(gg.REGION_C_ALLOC)
gg.searchNumber("67109633", gg.TYPE_DWORD)
if gg.getResultCount() <= 3 then
gg.alert("ANTI CHEAT RESULTS: "..gg.getResultCount().."\nSTATUS: SAFE")
gg.clearResults()
else
if gg.getResultCount() <= 7 and gg.getResultCount() >= 3 then
gg.alert("ANTI CHEAT RESULTS: "..gg.getResultCount().."\nSTATUS: RISK")
gg.clearResults()
else
omid = gg.alert("ANTI CHEAT RESULTS: "..gg.getResultCount().."\nSTATUS: BAN\nاگه ریزالت بای پس بالای 1000 باشه یعنی بای پس رو درست نزدی❌️❌️","EXIT", "CONTINUE")
if omid == 1 then
gg.processKill()
os.exit()
end
if omid == 2 then
home()
end
end
gg.clearResults()
end
end

function antibancheker()
gg.setRanges(gg.REGION_C_ALLOC)
gg.searchNumber("7959267916447219712", gg.TYPE_QWORD)
if gg.getResultCount() >= 350 then
gg.alert("آنتی بن درست فعال شده است✅️❤️")
else
omid = gg.alert("آنتی بن درست فعال نشده است❌️","EXIT", "CONTINUE")
if omid == 1 then
gg.processKill()
os.exit()
end
if omid == 2 then
home()
end
end
gg.clearResults()
end

function report()
gg.setRanges(gg.REGION_CODE_APP)
gg.processResume()
gg.searchNumber(":e AnoSDKInit", gg.TYPE_BYTE, false, gg.SIGN_EQUAL, 0, -1, 0)

revert = gg.getResults(50000, nil, nil, nil, nil, nil, nil, nil, nil)
local t = gg.getResults(50000, nil, nil, nil, nil, nil, nil, nil, nil)
for i, v in ipairs(t) do
	if v.flags == gg.TYPE_BYTE then
		v.value = "-1"
		v.freeze = true
	end
end
gg.addListItems(t)
t = nil


gg.clearResults()

gg.clearList()
gg.processResume()
gg.searchNumber(": AnoSDKDelReportData", gg.TYPE_BYTE, false, gg.SIGN_EQUAL, 0, -1, 0)

revert = gg.getResults(50000, nil, nil, nil, nil, nil, nil, nil, nil)
local t = gg.getResults(50000, nil, nil, nil, nil, nil, nil, nil, nil)
for i, v in ipairs(t) do
	if v.flags == gg.TYPE_BYTE then
		v.value = "-1"
		v.freeze = true
	end
end
gg.addListItems(t)
t = nil


gg.clearResults()

gg.clearList()
gg.processResume()
gg.searchNumber(":AnoSDKGetReportData3", gg.TYPE_BYTE, false, gg.SIGN_EQUAL, 0, -1, 0)

revert = gg.getResults(50000, nil, nil, nil, nil, nil, nil, nil, nil)
local t = gg.getResults(50000, nil, nil, nil, nil, nil, nil, nil, nil)
for i, v in ipairs(t) do
	if v.flags == gg.TYPE_BYTE then
		v.value = "-1"
		v.freeze = true
	end
end
gg.addListItems(t)
t = nil


gg.clearResults()

gg.clearList()
gg.processResume()
gg.setRanges(gg.REGION_CODE_APP)
gg.processResume()
gg.searchNumber(": AnoSDKDelReportData3 An", gg.TYPE_BYTE, false, gg.SIGN_EQUAL, 0, -1, 0)
gg.processResume()
gg.setRanges(gg.REGION_CODE_APP)
gg.searchNumber(":oSDKGetReportData2 A", gg.TYPE_BYTE, false, gg.SIGN_EQUAL, 0, -1, 0)

revert = gg.getResults(50000, nil, nil, nil, nil, nil, nil, nil, nil)
local t = gg.getResults(50000, nil, nil, nil, nil, nil, nil, nil, nil)
for i, v in ipairs(t) do
	if v.flags == gg.TYPE_BYTE then
		v.value = "-1"
		v.freeze = true
	end
end
gg.addListItems(t)
t = nil


gg.clearResults()

gg.clearList()
gg.processResume()
gg.searchNumber(":noSDKForExport AnoSDKGetReportData A", gg.TYPE_BYTE, false, gg.SIGN_EQUAL, 0, -1, 0)

revert = gg.getResults(50000, nil, nil, nil, nil, nil, nil, nil, nil)
local t = gg.getResults(50000, nil, nil, nil, nil, nil, nil, nil, nil)
for i, v in ipairs(t) do
	if v.flags == gg.TYPE_BYTE then
		v.value = "-1"
		v.freeze = true
	end
end
gg.addListItems(t)
t = nil


gg.clearResults()

gg.clearList()
gg.processResume()
gg.setRanges(gg.REGION_CODE_APP)
gg.processResume()
gg.searchNumber(":noSDKFree An", gg.TYPE_BYTE, false, gg.SIGN_EQUAL, 0, -1, 0)

revert = gg.getResults(50000, nil, nil, nil, nil, nil, nil, nil, nil)
local t = gg.getResults(50000, nil, nil, nil, nil, nil, nil, nil, nil)
for i, v in ipairs(t) do
	if v.flags == gg.TYPE_BYTE then
		v.value = "-1"
		v.freeze = true
	end
end
gg.addListItems(t)
t = nil


gg.clearResults()

gg.clearList()
gg.setRanges(gg.REGION_CODE_APP)
gg.processResume()
gg.searchNumber(":oSDKSetUserInfo", gg.TYPE_BYTE, false, gg.SIGN_EQUAL, 0, -1, 0)

revert = gg.getResults(50000, nil, nil, nil, nil, nil, nil, nil, nil)
local t = gg.getResults(50000, nil, nil, nil, nil, nil, nil, nil, nil)
for i, v in ipairs(t) do
	if v.flags == gg.TYPE_BYTE then
		v.value = "-1"
		v.freeze = true
	end
end
gg.addListItems(t)
t = nil


gg.clearResults()

gg.clearList()
gg.setRanges(gg.REGION_CODE_APP)
gg.processResume()
gg.searchNumber(":AnoSDKIoctl", gg.TYPE_BYTE, false, gg.SIGN_EQUAL, 0, -1, 0)

revert = gg.getResults(50000, nil, nil, nil, nil, nil, nil, nil, nil)
local t = gg.getResults(50000, nil, nil, nil, nil, nil, nil, nil, nil)
for i, v in ipairs(t) do
	if v.flags == gg.TYPE_BYTE then
		v.value = "-1"
		v.freeze = true
	end
end
gg.addListItems(t)
t = nil


gg.clearResults()

gg.clearList()
gg.processResume()
gg.setRanges(gg.REGION_CODE_APP)
gg.processResume()
gg.searchNumber(":AnoSDKRegistInfoListener", gg.TYPE_BYTE, false, gg.SIGN_EQUAL, 0, -1, 0)

revert = gg.getResults(50000, nil, nil, nil, nil, nil, nil, nil, nil)
local t = gg.getResults(50000, nil, nil, nil, nil, nil, nil, nil, nil)
for i, v in ipairs(t) do
	if v.flags == gg.TYPE_BYTE then
		v.value = "-1"
		v.freeze = true
	end
end
gg.addListItems(t)
t = nil


gg.clearResults()

gg.clearList()
gg.setRanges(gg.REGION_CODE_APP)
gg.processResume()
gg.searchNumber(": AnoSDKIoctlOld", gg.TYPE_BYTE, false, gg.SIGN_EQUAL, 0, -1, 0)
gg.setRanges(gg.REGION_CODE_APP)
gg.processResume()
gg.searchNumber(":AnoSDKOnResume A", gg.TYPE_BYTE, false, gg.SIGN_EQUAL, 0, -1, 0)

revert = gg.getResults(50000, nil, nil, nil, nil, nil, nil, nil, nil)
local t = gg.getResults(50000, nil, nil, nil, nil, nil, nil, nil, nil)
for i, v in ipairs(t) do
	if v.flags == gg.TYPE_BYTE then
		v.value = "-1"
		v.freeze = true
	end
end
gg.addListItems(t)
t = nil


gg.clearResults()

gg.clearList()
gg.processResume()
gg.searchNumber(":noSDKOnPause", gg.TYPE_BYTE, false, gg.SIGN_EQUAL, 0, -1, 0)

revert = gg.getResults(50000, nil, nil, nil, nil, nil, nil, nil, nil)
local t = gg.getResults(50000, nil, nil, nil, nil, nil, nil, nil, nil)
for i, v in ipairs(t) do
	if v.flags == gg.TYPE_BYTE then
		v.value = "-1"
		v.freeze = true
	end
end
gg.addListItems(t)
t = nil


gg.clearResults()

gg.clearList()
gg.setRanges(gg.REGION_CODE_APP)
gg.processResume()
gg.searchNumber(": AnoSDKOnRecvSignature A", gg.TYPE_BYTE, false, gg.SIGN_EQUAL, 0, -1, 0)

revert = gg.getResults(50000, nil, nil, nil, nil, nil, nil, nil, nil)
local t = gg.getResults(50000, nil, nil, nil, nil, nil, nil, nil, nil)
for i, v in ipairs(t) do
	if v.flags == gg.TYPE_BYTE then
		v.value = "-1"
		v.freeze = true
	end
end
gg.addListItems(t)
t = nil


gg.clearResults()

gg.clearList()
gg.setRanges(gg.REGION_CODE_APP)
gg.processResume()
gg.searchNumber(":noSDKOnRecvData", gg.TYPE_BYTE, false, gg.SIGN_EQUAL, 0, -1, 0)

revert = gg.getResults(50000, nil, nil, nil, nil, nil, nil, nil, nil)
local t = gg.getResults(50000, nil, nil, nil, nil, nil, nil, nil, nil)
for i, v in ipairs(t) do
	if v.flags == gg.TYPE_BYTE then
		v.value = "-1"
		v.freeze = true
	end
end
gg.addListItems(t)
t = nil


gg.clearResults()
gg.processResume()
gg.clearList()
gg.setRanges(gg.REGION_CODE_APP)
gg.processResume()
gg.searchNumber(":ClearReport", gg.TYPE_BYTE, false, gg.SIGN_EQUAL, 0, -1, 0)

revert = gg.getResults(50000, nil, nil, nil, nil, nil, nil, nil, nil)
local t = gg.getResults(50000, nil, nil, nil, nil, nil, nil, nil, nil)
for i, v in ipairs(t) do
	if v.flags == gg.TYPE_BYTE then
		v.value = "0"
		v.freeze = true
	end
end
gg.addListItems(t)
t = nil
gg.clearResults()
gg.processResume()
gg.clearList()
gg.alert("ANTI REPORT ACTIVATED✅️❤️")
end

function labychits()
OMIDSEIFI= gg.multiChoice({
"Aimbot",
"Wallhack",
"Red Line",
"No Spread",
"Fast Scoob",
"Fast Switch",
"No Reloead",
"Crosshair",
"Magic Test",
"Back",
}, nil, os.date("%A %d %B %T %Y/%m/%d"))
if OMIDSEIFI == nil then else
if OMIDSEIFI [1] == true then aim()end
if OMIDSEIFI [2] == true then wall()end
if OMIDSEIFI [3] == true then redline()end
if OMIDSEIFI [4] == true then no()end
if OMIDSEIFI [5] == true then fast()end
if OMIDSEIFI [6] == true then switch()end
if OMIDSEIFI [7] == true then reload()end
if OMIDSEIFI [8] == true then cro()end
if OMIDSEIFI [9] == true then testmagic()end
if OMIDSEIFI [10] == true then home()end
end
OMIDSEIFI= 1
end

function aim()
so = gg.getRangesList('libil2cpp.so')[1].start
py = 0x9f96aa80
setvalue(so + py, 16, 500.0)
gg.toast("AIM BOT ACTIVATED✅❤️")
end

function wall()
--WALL HACK
so=gg.getRangesList('libil2cpp.so')[1].start
py=0x1a4e6f4
setvalue(so+py,4,0)
--ESP
so=gg.getRangesList('libil2cpp.so')[1].start
py=0x18c5d6c
setvalue(so+py,4,3818913793.0)

so=gg.getRangesList('libil2cpp.so')[1].start
py=0x18c5d70
setvalue(so+py,4,3778019102.0)
gg.toast("ᴇꜱᴘ ɴᴀᴍᴇ ʙʀ ᴏɴ")
gg.toast("WALL HACK ACTIVATED✅❤️")
end

function redline()
gg.setRanges(gg.REGION_ANONYMOUS)
gg.searchNumber("4575657222490554368;1065353216:9", gg.TYPE_QWORD, false, gg.SIGN_EQUAL, 0, -1, 0)
gg.refineNumber("4575657222490554368;1065353216", gg.TYPE_QWORD, false, gg.SIGN_EQUAL, 0, -1, 0)
gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("4575657222520438784;1133903872", gg.TYPE_QWORD)
gg.clearResults()
gg.toast("RED LINE ACTIVATED✅❤️")
end

function cro()
gg.setRanges(gg.REGION_ANONYMOUS)
gg.searchNumber("4;5;6;7", gg.TYPE_FLOAT)
gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("-500", gg.TYPE_FLOAT)
gg.clearResults()
gg.toast("CROOS HAIR ACTIVATED✅❤️")
end

function no()
so=gg.getRangesList('libil2cpp.so')[1].start
py=0x2fc857c
setvalue(so+py,4,3812821656.0)
so=gg.getRangesList('libil2cpp.so')[1].start
py=0x2fc8580
setvalue(so+py,4,3778019102.0)
gg.toast("NO SPREAD ACTIVATED✅❤️")
end

function fast()
so=gg.getRangesList('libil2cpp.so')[1].start
py=0x19caaa4
setvalue(so+py,4,-442564608)
so=gg.getRangesList('libil2cpp.so')[1].start
py=0x19caaa8
setvalue(so+py,4,-516948194)
so=gg.getRangesList('libil2cpp.so')[1].start
py=0x19caaac
setvalue(so+py,4,981668463)
gg.toast("FAST SCOBE ACTIVATED✅❤️")
end

function switch()
so=gg.getRangesList('libil2cpp.so')[1].start  
py=0x1B2FD90 
setvalue(so+py,4,-482145640)
so=gg.getRangesList('libil2cpp.so')[1].start  
py=0x1B2FD94 
setvalue(so+py,4,-516948194)
so=gg.getRangesList('libil2cpp.so')[1].start  
py=0x1B2FFEC 
setvalue(so+py,4,-482145640)
so=gg.getRangesList('libil2cpp.so')[1].start  
py=0x1B2FFF0 
setvalue(so+py,4,-516948194)
gg.toast("FAST SWITCH ACTIVATED✅❤️")
end

function reload()
gg.setRanges(gg.REGION_ANONYMOUS)
gg.searchNumber("1,062,897,032;1,059,313,418;1,067,366,482;1,062,897,032", gg.TYPE_DWORD, false, gg.SIGN_EQUAL, 0, -1, 0)
gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("999", gg.TYPE_DWORD)
gg.clearResults()
gg.toast("NO RELOEAD ACTIVATED✅❤️")
end

function amoo2()
gg.alert("باید ۳۰ تا تیر داشته باشه")
gg.setRanges(gg.REGION_ANONYMOUS)
gg.searchNumber("90;30;1;0:25", gg.TYPE_DWORD, false, gg.SIGN_EQUAL, 0, -1, 0)
revert = gg.getResults(50)
local t = gg.getResults(50)
for i, v in ipairs(t) do
	if v.flags == gg.TYPE_DWORD then
		v.value = "9999"
		v.freeze = true
	end
end
gg.addListItems(t)
t = nil
gg.clearResults()
gg.alert("AMOO UNLIMITED GUN ACTIVATED✅❤️")
end

function amoo3()
gg.alert("باید ۵ تا تیر داشته باشه")
gg.setRanges(gg.REGION_ANONYMOUS)
gg.searchNumber("15;5;1;0:25", gg.TYPE_DWORD, false, gg.SIGN_EQUAL, 0, -1, 0)
revert = gg.getResults(50)
local t = gg.getResults(50)
for i, v in ipairs(t) do
	if v.flags == gg.TYPE_DWORD then
		v.value = "99999"
		v.freeze = true
	end
end
gg.addListItems(t)
t = nil
gg.clearResults()
gg.alert("AMOO UNLIMITED SNAIPE ACTIVATED✅❤️")
end

function testmagic()
gg.setRanges(gg.REGION_ANONYMOUS)
--gg.searchNumber("0.00999999978;0.03999999911~0.60000002384;0.10000000149~0.5;12::53"gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1)
gg.searchNumber("0.03999999911~0.60000002384", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1)
gg.getResults(6000)
gg.editAll("1.1439999938", gg.TYPE_FLOAT)
gg.toast("Magic Test ACTIVATED✅❤️")
end

function gamechits()
OMIDSEIFI= gg.multiChoice({
"More...",
"Magic Bullt",
"Head Shot",
"Wall Shot",
"Fast Shot",
"No Recoil",
"Hack Gravity",
"Black Track",
"No Smoke",
"Slide Hack",
"High Jump",
"IPad View",
"Speed ​​Hack",
"Antenna",
"Game Speed",
"Back",
}, nil, os.date("%A %d %B %T %Y/%m/%d"))
if OMIDSEIFI == nil then else
if OMIDSEIFI [1] == true then more()end
if OMIDSEIFI [2] == true then magic()end
if OMIDSEIFI [3] == true then shot1()end
if OMIDSEIFI [4] == true then shot()end
if OMIDSEIFI [5] == true then fastshot()end
if OMIDSEIFI [6] == true then recoil()end
if OMIDSEIFI [7] == true then gravity()end
if OMIDSEIFI [8] == true then bullet()end
if OMIDSEIFI [9] == true then smoc()end
if OMIDSEIFI [10] == true then slide()end
if OMIDSEIFI [11] == true then jamp()end
if OMIDSEIFI [12] == true then ipad()end
if OMIDSEIFI [13] == true then speed()end
if OMIDSEIFI [14] == true then antenna()end
if OMIDSEIFI [15] == true then gamespeed()end
if OMIDSEIFI [16] == true then home()end
end
OMIDSEIFI= 1
end

function magic()
function setvalue(address,flags,value)
 local tt={} tt[1]={} tt[1].address=address tt[1].flags=flags tt[1].value=value gg.setValues(tt) end
omidseifi = gg.alert("Magic bullt", "Head", "Bady")
if omidseifi == 1 then
gg.setRanges(gg.REGION_ANONYMOUS)
gg.searchNumber("0.1439999938", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1)
gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("0.80", gg.TYPE_FLOAT)
gg.clearResults()
gg.toast("Magic bullt Head ACTIVATED✅❤️")
else
if omidseifi == 2 then
gg.setRanges(gg.REGION_ANONYMOUS)
gg.searchNumber("0.18500000238", gg.TYPE_FLOAT)
gg.refineNumber("0.18500000238", gg.TYPE_FLOAT)
gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("2.5", gg.TYPE_FLOAT)
gg.clearResults()
gg.setRanges(gg.REGION_ANONYMOUS)
gg.searchNumber("0.18500000238", gg.TYPE_FLOAT)
gg.refineNumber("0.18500000238", gg.TYPE_FLOAT)
gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("2.5", gg.TYPE_FLOAT)
gg.clearResults()
gg.setRanges(gg.REGION_ANONYMOUS)
gg.searchNumber("0.18500000238", gg.TYPE_FLOAT)
gg.refineNumber("0.18500000238", gg.TYPE_FLOAT)
gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("2.5", gg.TYPE_FLOAT)
gg.clearResults()
gg.setRanges(gg.REGION_ANONYMOUS)
gg.searchNumber("0.18500000238", gg.TYPE_FLOAT)
gg.refineNumber("0.18500000238", gg.TYPE_FLOAT)
gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("2.5", gg.TYPE_FLOAT)
gg.clearResults()
gg.toast("Magic bullt Bady ACTIVATED✅❤️")
return
end
end
end


function shot1()
gg.setRanges(gg.REGION_ANONYMOUS)
gg.searchNumber("1041462460", gg.TYPE_DWORD)
gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("1077936128", gg.TYPE_DWORD)
gg.clearResults()
gg.toast("Head Shot ACTIVATED✅❤️")
end

function shot()
gg["setRanges"](gg["REGION_C_BSS"])
gg["searchNumber"]("2", gg["TYPE_FLOAT"], false, gg["SIGN_EQUAL"], 0, -1, 0)
gg["getResults"](100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg["editAll"]("-999", gg["TYPE_FLOAT"])
gg.toast("Wall Shot ACTIVATED✅❤️")
end

function fastshot()
so = gg.getRangesList("libil2cpp.so")[1].start
py = 32817172
setvalue(so + py, 4, 0)
so = gg.getRangesList("libil2cpp.so")[1].start
py = 32824336
setvalue(so + py, 4, 0)
gg.clearResults()
gg.toast("Fast Shot ACTIVATED✅❤️")
end

function recoil()
gg.setRanges(gg.REGION_ANONYMOUS)
gg.searchNumber("13;9;1", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1, 0)
gg.refineNumber("1", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1, 0)
gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("9.99999968e-22", gg.TYPE_FLOAT)
gg.clearResults()
gg.toast("No Recoil ACTIVATED✅❤️")
end

function gravity()
--HACK GRAVITY
gg.setRanges(gg.REGION_ANONYMOUS)
gg.searchNumber("-1,063,172,178", gg.TYPE_DWORD, false, gg.SIGN_EQUAL, 0, -1, 0)
gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("99", gg.TYPE_DWORD)
gg.clearResults()
gg.toast("HACK GRAVITY ACTIVATED✅❤️")
end

function bullet()
omidseifi = gg.alert("bullet Track", "V1", "V2")
if omidseifi == 1 then
so = gg.getRangesList('libunity.so')[1].start
py = 0x511EF8
setvalue(so+py,16,9)
so = gg.getRangesList('libunity.so')[1].start
py = 0xb30418
setvalue(so+py,16,23)
so = gg.getRangesList('libunity.so')[1].start
py = 0xb3041c
setvalue(so+py,16,23)
so = gg.getRangesList('libunity.so')[1].start
py = 0xb307b4
setvalue(so+py,16,0)
so = gg.getRangesList('libunity.so')[1].start
py = 0xb307d4
setvalue(so+py,16,0)
so = gg.getRangesList('libunity.so')[1].start
py = 0xb307d8
setvalue(so+py,16,0)
so = gg.getRangesList('libunity.so')[1].start
py = 0xb307dc
setvalue(so+py,16,0)
so = gg.getRangesList('libunity.so')[1].start
py = 0xb308f4
setvalue(so+py,16,0)
so = gg.getRangesList('libunity.so')[1].start
py = 0xb30a38
setvalue(so+py,16,23)
so = gg.getRangesList('libunity.so')[1].start
py = 0xb30a3c
setvalue(so+py,16,0)
gg.toast("Bullet Track V1 ACTIVATED✅❤️")
else
if omidseifi == 2 then
so = gg.getRangesList("libunity.so")[1].start
py = 0x511ef8
setvalue(so + py, 4, 1098697933)
gg.toast("Bullet Track V2 ACTIVATED✅❤️")
return
end
end
end

function smoc()
gg.setRanges(gg.REGION_ANONYMOUS)
gg.searchNumber("300000090",gg.TYPE_DWORD)
gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("0",gg.TYPE_DWORD)
gg.clearResults()
gg.toast("No Smoce ACTIVATED✅❤️")
end

function slide()
so=gg.getRangesList('libil2cpp.so')[1].start
py=0x1e605a0     
setvalue(so+py,4,3812885192.0)
so=gg.getRangesList('libil2cpp.so')[1].start
py=0x1e605a4     
setvalue(so+py,4,3778019102.0)
gg.toast("Slide Hack ACTIVATED✅❤️")
end

function jamp()
gg.setRanges(gg.REGION_ANONYMOUS)
gg.searchNumber("7.5;0.8::5", gg.TYPE_FLOAT)
gg.refineNumber("0.8", gg.TYPE_FLOAT)
gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("999", gg.TYPE_FLOAT)
gg.clearResults()
gg.toast("Jamp Hack MP ACTIVATED✅❤️")
gg.setRanges(gg.REGION_ANONYMOUS)
gg.searchNumber("1,065,353,216;1,069,547,520;1,050,253,722:9", gg.TYPE_DWORD)
gg.refineNumber("1,065,353,216", gg.TYPE_DWORD)
gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("1,082,130,432", gg.TYPE_DWORD)
gg.clearResults()
gg.toast("Jamp Hack BR ACTIVATED✅❤️")
end

function ipad()
gg.setRanges(gg.REGION_ANONYMOUS)
gg.searchNumber("44.0;44.0;60.0;45.0;0.20000000298:33", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0,-1)
gg.searchNumber("44", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1)
gg.getResults("950")
gg.editAll("98", gg.TYPE_FLOAT)
gg.clearResults()
gg.toast("آیپد ویو با موفقیت فعال شد.✅️")
end


function speed()
gg.setRanges(gg.REGION_ANONYMOUS)
Y=math.random(1,15) 
V=gg.prompt({"🏃🏻میزان سرعت دویدن را انتخاب کنید.🏃🏻‍♀[1;15]"},{Y},{"number","checkbox"})
for i = 1,5 do gg.sleep(10) gg.setVisible(false) gg.toast("شروع هک میزان سرعت دویدن: "..V[1]) end
if V[2] == true then
gg.searchNumber("4.28000020981;3.20000004768;0.30000001192;0.20000000298", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1)
else
gg.searchNumber("4.28000020981;3.20000004768;0.30000001192;0.20000000298", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1)
end
-------------------------------(NoLag_Test)------------------------
speedmenubar=tonumber(V[1]) 
---------------------------------------------------------------------------
if speedmenubar == 1 then
Speed = gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("2", gg.TYPE_FLOAT)
gg.clearResults()
gg.alert("هک راه رفتن سطح 1 با موفقیت فعال شد.✅")
else
end
if speedmenubar == 2 then
Speed = gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("3", gg.TYPE_FLOAT)
gg.clearResults()
gg.alert("هک راه رفتن سطح 2 با موفقیت فعال شد.✅")
else
end
if speedmenubar == 3 then
Speed = gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("4", gg.TYPE_FLOAT)
gg.clearResults()
gg.toast("هک راه رفتن سطح 3 با موفقیت فعال شد.✅")
else
end
if speedmenubar == 4 then
Speed = gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("5", gg.TYPE_FLOAT)
gg.clearResults()
gg.toast("هک راه رفتن سطح 4 با موفقیت فعال شد.✅")
else
end
if speedmenubar == 5 then
Speed = gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("6", gg.TYPE_FLOAT)
gg.clearResults()
gg.toast("هک راه رفتن سطح 5 با موفقیت فعال شد.✅")
else
end
if speedmenubar == 6 then
Speed = gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("7", gg.TYPE_FLOAT)
gg.clearResults()
gg.toast("هک راه رفتن سطح 6 با موفقیت فعال شد.✅")
else
end
if speedmenubar == 7 then
Speed = gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("8", gg.TYPE_FLOAT)
gg.clearResults()
gg.toast("هک راه رفتن سطح 7 با موفقیت فعال شد.✅")
else
end
if speedmenubar == 8 then
Speed = gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("9", gg.TYPE_FLOAT)
gg.clearResults()
gg.toast("هک راه رفتن سطح 8 با موفقیت فعال شد.✅")
else
end
if speedmenubar == 9 then
Speed = gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("10", gg.TYPE_FLOAT)
gg.clearResults()
gg.toast("هک راه رفتن سطح 9 با موفقیت فعال شد.✅")
else
end
if speedmenubar == 10 then
Speed = gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("11", gg.TYPE_FLOAT)
gg.clearResults()
gg.toast("هک راه رفتن سطح 10 با موفقیت فعال شد.✅")
else
end
if speedmenubar == 11 then
Speed = gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("12", gg.TYPE_FLOAT)
gg.clearResults()
gg.toast("هک راه رفتن سطح 11 با موفقیت فعال شد.✅")
else
end
if speedmenubar == 12 then
Speed = gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("13", gg.TYPE_FLOAT)
gg.clearResults()
gg.toast("هک راه رفتن سطح 12 با موفقیت فعال شد.✅")
else
end
if speedmenubar == 13 then
Speed = gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("14", gg.TYPE_FLOAT)
gg.clearResults()
gg.toast("هک راه رفتن سطح 13 با موفقیت فعال شد.✅")
else
end
if speedmenubar == 14 then
Speed = gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("15", gg.TYPE_FLOAT)
gg.clearResults()
gg.toast("هک راه رفتن سطح 14 با موفقیت فعال شد.✅")
else
end
if speedmenubar == 15 then
Speed = gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("9999999999999999", gg.TYPE_FLOAT)
gg.clearResults()
gg.toast("هک راه رفتن سطح 15 با موفقیت فعال شد.✅")
end
end


function antenna()
gg.setRanges(gg.REGION_ANONYMOUS)
gg.searchNumber("1.0193~1.0194", gg.TYPE_FLOAT)
gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("100", gg.TYPE_FLOAT)
gg.clearResults()
gg.setRanges(gg.REGION_ANONYMOUS)
gg.searchNumber("1.5~1.6;0.2~0.22::5", gg.TYPE_FLOAT)
gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("-100", gg.TYPE_FLOAT)
gg.clearResults()
gg.toast("Antenna ACTIVATED✅❤️")
end

function gamespeed()
gg.setRanges(gg.REGION_ANONYMOUS)
Y=math.random(1,10) 
V=gg.prompt({"میزان اسپید بازی را انتخاب نمایید.[1;10]"},{Y},{"number"})

gamespeed=tonumber(V[1])

if gamespeed == 1 then
gg.searchNumber("0.99999988079F;1.0F;0.10000000149F;0.5F:100", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1)
gg.refineNumber("1", gg.TYPE_FLOAT)
gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("1.5", gg.TYPE_FLOAT)
gg.clearResults()
gg.alert("هک اسپید بازی سطح 1 با موفقیت فعال شد.✅")
else
end
if gamespeed == 2 then
gg.searchNumber("0.99999988079F;1.0F;0.10000000149F;0.5F:100", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1)
gg.refineNumber("1", gg.TYPE_FLOAT)
gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("2.5", gg.TYPE_FLOAT)
gg.clearResults()
gg.alert("هک اسپید بازی سطح 2 با موفقیت فعال شد.✅")
else
end
if gamespeed == 3 then
gg.searchNumber("0.99999988079F;1.0F;0.10000000149F;0.5F:100", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1)
gg.refineNumber("1", gg.TYPE_FLOAT)
gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("3", gg.TYPE_FLOAT)
gg.clearResults()
gg.toast("هک اسپید بازی سطح 3 با موفقیت فعال شد.✅")
else
end
if gamespeed == 4 then
gg.searchNumber("0.99999988079F;1.0F;0.10000000149F;0.5F:100", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1)
gg.refineNumber("1", gg.TYPE_FLOAT)
gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("4", gg.TYPE_FLOAT)
gg.clearResults()
gg.toast("هک اسپید بازی سطح 4 با موفقیت فعال شد.✅")
else
end
if gamespeed == 5 then
gg.searchNumber("0.99999988079F;1.0F;0.10000000149F;0.5F:100", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1)
gg.refineNumber("1", gg.TYPE_FLOAT)
gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("5", gg.TYPE_FLOAT)
gg.clearResults()
gg.toast("هک اسپید بازی سطح 5 با موفقیت فعال شد.✅")
else
end
if gamespeed == 6 then
gg.searchNumber("0.99999988079F;1.0F;0.10000000149F;0.5F:100", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1)
gg.refineNumber("1", gg.TYPE_FLOAT)
gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("5.5", gg.TYPE_FLOAT)
gg.clearResults()
gg.toast("هک اسپید بازی سطح 6 با موفقیت فعال شد.✅")
else
end
if gamespeed == 7 then
gg.searchNumber("0.99999988079F;1.0F;0.10000000149F;0.5F:100", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1)
gg.refineNumber("1", gg.TYPE_FLOAT)
gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("6", gg.TYPE_FLOAT)
gg.clearResults()
gg.toast("هک اسپید بازی سطح 7 با موفقیت فعال شد.✅")
else
end
if gamespeed == 8 then
gg.searchNumber("0.99999988079F;1.0F;0.10000000149F;0.5F:100", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1)
gg.refineNumber("1", gg.TYPE_FLOAT)
gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("6.5", gg.TYPE_FLOAT)
gg.clearResults()
gg.toast("هک اسپید بازی سطح 8 با موفقیت فعال شد.✅")
else
end
if gamespeed == 9 then
gg.searchNumber("0.99999988079F;1.0F;0.10000000149F;0.5F:100", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1)
gg.refineNumber("1", gg.TYPE_FLOAT)
gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("7", gg.TYPE_FLOAT)
gg.clearResults()
gg.toast("هک اسپید بازی سطح 9 با موفقیت فعال شد.✅")
else
end
if gamespeed == 10 then
gg.searchNumber("0.99999988079F;1.0F;0.10000000149F;0.5F:100", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1)
gg.refineNumber("1", gg.TYPE_FLOAT)
gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("7.5", gg.TYPE_FLOAT)
gg.clearResults()
gg.toast("هک اسپید بازی سطح 10 با موفقیت فعال شد.✅")
end
end


function more()
OMIDSEIFI = gg.multiChoice({
"Bady Gint",
"Black Sky",
"Back",
}, nil, os.date("%A %d %B %T %Y/%m/%d"))
if OMIDSEIFI == nil then else
if OMIDSEIFI [1] == true then badygint()end
if OMIDSEIFI [2] == true then blacksky()end
if OMIDSEIFI [3] == true then gamechits()end
end
OMIDSEIFI= 1
end


function badygint()
--BODY GINT
gg.setRanges(gg.REGION_ANONYMOUS)
gg.searchNumber("1067534200D~3000000000D;-0;0.1~0.99;1;1;1::37", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1, 0)
gg.refineNumber("1", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1, 0)
gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("-3.5", gg.TYPE_FLOAT)
gg.clearResults()
gg.toast("BODY GINT ACTIVATED✅❤️")
end



function blacksky()
--BLACK SKY
gg.setRanges(gg.REGION_ANONYMOUS)
gg.searchNumber("1048592;1048596;1048680;1048700", gg.TYPE_DWORD, false, gg.SIGN_EQUAL, 0, -1, 0)
gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
gg.editAll("0", gg.TYPE_DWORD)
gg.clearResults()
gg.toast("BLACK SKY ACTIVATED✅❤️")
end

function EXIT1()
os.exit()
end



while true do
  if gg.isVisible(true) then
MenU = 1
gg.setVisible(false)
  end
if MenU == 1 then
home()
  end
  end
