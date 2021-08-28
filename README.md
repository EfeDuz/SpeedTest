import speedtest

s = speedtest.Speedtest()
print("Test Yapılıyor... /n")






ındırmehızı = s.download() / 1048576
yuklemehızı = s.upload() / 1048576
ping = round(s.results.ping)

print(f"İndirme Hızı = {ındırmehızı:.2f} Mbps    ")
print(f"Yükleme Hızı = {yuklemehızı:.2f} Mbps    ")
print(f"Ping = {ping:.2f} ms    ")

