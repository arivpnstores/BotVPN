## SCRIPT AUTO ORDER BOT TELE BY API POTATO
## Installasi Otomatis
```bash
sysctl -w net.ipv6.conf.all.disable_ipv6=1 && sysctl -w net.ipv6.conf.default.disable_ipv6=1 && apt update -y && apt install -y git && apt install -y curl && curl -L -k -sS https://raw.githubusercontent.com/arivpnstores/BotVPN/main/start -o start && bash start sellvpn && [ $? -eq 0 ] && rm -f start
```
## UPDATE
```bash
curl -sSL https://raw.githubusercontent.com/arivpnstores/BotVPN/main/update.sh -o update.sh && chmod +x update.sh && bash update.sh
```
<img src="./ss.png" alt="image" width="500"/>

## DATA QRIS DI DAPAT KAN DARI FOTO QRIS ORDER KUOTA
https://qreader.online/

## CEK PEMBAYARAN 
EDIT FILE DI api-cekpayment-orkut.js
TUTORIAL AMBIL API CEK PEMBAYARAN VIA VIDIO : https://drive.google.com/file/d/1ugR_N5gEtcLx8TDsf7ecTFqYY3zrlHn-/view?usp=drivesdk
TANYA CHAT GPT GINI!!!!
```bash
ubah data senif ini
 POST https://app.orderkuota.com/api/v2/qris/mutasi/4xxxxx HTTP/2.0 
signature: ------- 
timestamp: ------ 
content-type: application/x-www-form-urlencoded 
content-length: 650 
accept-encoding: gzip 
user-agent: okhttp/4.12.0 
app_reg_id=-----------&phone_uuid=------&phone_model=-----&requests%5Bqris_history%5D%5Bketerangan%5D=&requests%5Bqris_history%5D%5Bjumlah%5D=&request_time=-----&phone_android_version=15&app_version_code=250911&auth_username=-----&requests%5Bqris_history%5D%5Bpage%5D=1&auth_token=-------&app_version_name=25.09.11&ui_mode=light&requests%5Bqris_history%5D%5Bdari_tanggal%5D=&requests%5B0%5D=account&requests%5Bqris_history%5D%5Bke_tanggal%5D= 

menjadi kayak gini 
// api-cekpayment-orkut.js
const qs = require('qs');

// Function agar tetap kompatibel dengan app.js
function buildPayload() {
  return qs.stringify({
    'username': 'yantoxxx',
    'token': '1342xxxx:149:i3NBVaZqHjEYnvuImxWKACgxxxxx',
    'jenis': 'masuk'
  });
}

// Header tetap sama agar tidak error di app.js
const headers = {
  'Content-Type': 'application/x-www-form-urlencoded',
  'Accept-Encoding': 'gzip',
  'User-Agent': 'okhttp/4.12.0'
};

// URL baru sesuai curl-mu
const API_URL = 'https://orkutapi.andyyuda41.workers.dev/api/qris-history';

// Ekspor agar app.js tetap bisa require dengan struktur lama
module.exports = { buildPayload, headers, API_URL };
```
ganti txt hasil seniff anda

## TAMPILAN SC BotVPN POTATO 
<img src="./ss2.png" alt="image" width="300"/>
kasih uang jajan : https://serverpremium.web.id/payment/

Owner : https://t.me/ARI_VPN_STORE
