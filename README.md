#!url=noturl
#!name=Locket-VuChiHuong_Gold
#!desc=Crack By VuChiHuong

[Script]
revenuecat = type=http-response, pattern=^https:\/\/api\.revenuecat\.com\/.+\/(receipts$|subscribers\/[^/]+$), script-path=https://raw.githubusercontent.com/nhdunx/Locket/refs/heads/main/Locket_DungMomx.js, requires-body=true, max-size=-1, timeout=60

deleteHeader = type=http-request, pattern=^https:\/\/api\.revenuecat\.com\/.+\/(receipts|subscribers), script-path=https://raw.githubusercontent.com/nhdunx/Locket/refs/heads/main/deleteHeader.js, timeout=60

[MITM]
hostname = %APPEND% api.revenuecat.com
