# بدون حقوق حط حقوقوك
import requests
import os
import sys
import time
import re
from random import randrange, choice
from user_agent import generate_user_agent
from concurrent.futures import ThreadPoolExecutor
import random
E = '\033[1;31m'
Y = '\033[1;33m'
Z = '\033[1;31m'
X = '\033[1;33m'
Z1 = '\033[2;31m'
F = '\033[2;32m'
A = '\033[2;34m'
C = '\033[2;35m'
S = '\033[2;36m'
G = '\033[1;34m'
HH = '\033[1;34m'
M = '\x1b[1;37m'
W1 = '\x1b[1;97m'
W2 = '\x1b[38;5;120m'
W3 = '\x1b[38;5;204m'
W4 = '\x1b[38;5;150m'
W5 = '\x1b[1;33m'
W6 = '\x1b[1;31m'
W7 = "\033[1;33m"
W8 = '\x1b[2;36m'
W8 = f'\x1b[38;5;117m'
W9 = "\033[1m\033[34m"
mlham = '\033[0m'
L = '\033[3;36m'
H = '\033[3;35m'
A1 = '\033[3;34m'
M1 = '\033[3;33m'
T = '\033[3;32m'
P='\x1b[38;5;231m'
J='\x1b[38;5;208m'
J1='\x1b[38;5;202m'
J2='\x1b[38;5;203m'
J21='\x1b[38;5;204m'
J22='\x1b[38;5;209m'
F1='\x1b[38;5;76m'
C1='\x1b[38;5;120m'
P1='\x1b[38;5;150m'
P2='\x1b[38;5;190m'
BR = '\x1b[38;5;208m'
AH2 = '\x1b[38;5;204m' 
AS2 = '\x1b[38;5;220m'
MJ = '\x1b[38;5;193m'
MJ2 = '\x1b[38;5;216m'
MJ3 = '\x1b[38;5;190m'
MJ4 = '\x1b[38;5;106m'
ma = '\x1b[38;5;26m'
c1 = '\x1b[38;5;120m'
j21 = '\x1b[38;5;204m'
p1 = '\x1b[38;5;150m'
cyan = "\033[1m\033[36m"
x = '\x1b[1;33m'
white = '\x1b[1;37m'
z = '\x1b[1;31m'
bi = random.randint(5,208)
ror1 = f'\x1b[38;5;{bi}m'
memo = random.randint(100, 300)
ror = f'\x1b[38;5;{memo}m'
P = '\x1b[38;5;231m'
J = '\x1b[38;5;208m'
J1 = '\x1b[38;5;202m'
J2 = '\x1b[38;5;203m'
J21 = '\x1b[38;5;204m'
J22 = '\x1b[38;5;209m'
F1 = '\x1b[38;5;76m'
C1 = '\x1b[38;5;120m'
P1 = '\x1b[38;5;150m'
P2 = '\x1b[38;5;190m'
BR = '\x1b[38;5;208m'
AH2 = '\x1b[38;5;204m'
AS2 = '\x1b[38;5;220m'
MJ = '\x1b[38;5;193m'
MJ2 = '\x1b[38;5;216m'
MJ3 = '\x1b[38;5;190m'
MJ4 = '\x1b[38;5;106m'
ma = '\x1b[38;5;26m'
E = '\033[1;31m'
Y = '\033[1;33m'
Z = '\033[1;31m'  # احمر
X = '\033[1;33m'  # اصفر
Z1 = '\033[2;31m'  # احمر ثاني
F = '\033[2;32m'  # اخضر
A = '\033[2;34m'  # ازرق
C = '\033[2;35m'  # وردي
S = '\033[2;36m'  # سمائي
G = '\033[1;34m'  # ازرق فاتح
HH = '\033[1;34m'  # ازرق فاتح
M = '\x1b[1;37m'  # ابيض
Y = "\033[1;33m"  # Yellow
R = '\033[1;31m'  # احمر
X = '\033[1;33m'  # اصفر
F = '\033[2;31m'  # اخضر
C = "\033[1;97m"  # ابيض
B = '\033[2;36m'  # سمائي
E = '\033[1;31m'
W9 = "\033[1m\033[34m"
M = '\x1b[1;37m'
HH = '\033[1;34m'
R = '\033[1;31;40m'
F = '\033[1;32;40m'
C = "\033[1;97;40m"
B = '\033[1;36;40m'
C1 = '\x1b[38;5;120m'
P1 = '\x1b[38;5;150m'
P2 = '\x1b[38;5;190m'
E = '\033[1;31m'
Y = '\033[1;33m'
Z = '\033[1;31m'
X = '\033[1;33m'
Z1 = '\033[2;31m'
F = '\033[2;32m'
A = '\033[2;34m'
C = '\033[2;35m'
S = '\033[2;36m'
red = "\033[1m\033[31m"
green = "\033[1m\033[32m"
yellow = "\033[1m\033[33m"
blue = "\033[1m\033[34m"
cyan = "\033[1m\033[36m"
magenta = "\033[1m\033[35m"
M = "\033[1m\033[36m"
white = "\033[1m\033[37m"
orange = "\033[1m\033[38;5;208m"
reset = "\033[0m"
a1 = '\x1b[1;31m'  # أح.مر
a2 = '\x1b[1;34m'  # أزرق
a3 = '\x1b[1;32m'  # أخضر
a4 = '\x1b[1;33m'  # أصفر
a5 = '\x1b[38;5;208m'  # برتقالي
a6 = '\x1b[38;5;5m'  # أرجواني
a7 = '\x1b[38;5;13m'  # وردي
a8 = '\x1b[1;30m'  # أسود
a9 = '\x1b[1;37m'  # أبيض
a10 = '\x1b[38;5;52m'  # بني
a11 = '\x1b[38;5;8m'  # رمادي
a12 = '\x1b[38;5;220m'  # ذهبي
a13 = '\x1b[38;5;7m'  # فضي
a14 = '\x1b[38;5;153m'  # أز.رق فاتح
a15 = '\x1b[38;5;18m'  # أزرق داكن
a16 = '\x1b[38;5;48m'  # أخضر فاتح
a17 = '\x1b[38;5;22m'  # أخض.ر داكن
a18 = '\x1b[38;5;196m'  # أحمر فاتح
a19 = '\x1b[38;5;88m'  # أحمر داكن
a20 = '\x1b[38;5;226m'  # أ.صفر فاتح
a21 = '\x1b[38;5;136m'  # أصفر داكن
a22 = '\x1b[38;5;216m'  # برتقالي فات
a23 = '\x1b[38;5;166m'  # برتقالي داكن
a24 = '\x1b[38;5;234m'  # أرجواني فاتح
a25 = '\x1b[38;5;91m'  # أرجواني داكن
a26 = '\x1b[38;5;205m'  # وردي فاتح
a27 = '\x1b[38;5;161m'  # وردي داكن
a28 = '\x1b[38;5;236m'  # أسود فاتح
a29 = '\x1b[38;5;233m'  # أسود داكن
a30 = '\x1b[38;5;255m'  # أبيض فاتح
a31 = '\x1b[38;5;231m'  # أبيض داكن
a32 = '\x1b[38;5;180m'  # بني فاتح
a33 = '\x1b[38;5;94m'  # بني داكن
a34 = '\x1b[38;5;252m'  # رمادي فاتح
a35 = '\x1b[38;5;246m'  # رمادي داكن
a36 = '\x1b[38;5;228m'  # ذهبي فاتح
a37 = '\x1b[38;5;172m'  # ذهبي داكن
a38 = '\x1b[38;5;188m'  # فضي فاتح
a39 = '\x1b[38;5;247m'  # فضي داكن
a40 = '\x1b[38;5;117m'  # أزرق سماوي
gg = '\x1b[38;5;208m'
X = '\033[1;33m'
J22 = '\x1b[38;5;209m'
J21 = '\x1b[38;5;204m'
J2 = '\x1b[38;5;203m'
J1 = '\x1b[38;5;202m'
E = '\033[1;31m'
W2 = '\x1b[38;5;120m'
W3 = '\x1b[38;5;204m'
W4 = '\x1b[38;5;150m'
W5 = '\x1b[1;33m'
W6 = '\x1b[1;31m'
W7 = "\033[1;33m"
W8 = '\x1b[2;36m'
W8 = f'\x1b[38;5;117m'
W9 = "\033[1m\033[34m"
P = '\x1b[1;97m'
B = '\x1b[1;94m'
O = '\x1b[1;96m'
Z = '\x1b[1;30m'
X = '\x1b[1;33m'
F = '\x1b[2;32m'
Z = '\x1b[1;31m'
L = '\x1b[1;95m'
C = '\x1b[2;35m'
A = '\x1b[2;39m'
P = '\x1b[38;5;231m'
J = '\x1b[38;5;208m'
J1 = '\x1b[38;5;202m'
J2 = '\x1b[38;5;203m'
J21 = '\x1b[38;5;204m'
J22 = '\x1b[38;5;209m'
F1 = '\x1b[38;5;76m'
C1 = '\x1b[38;5;120m'
P1 = '\x1b[38;5;150m'
P2 = '\x1b[38;5;190m'
E = '\033[1;31m'
Y = '\033[1;33m'
Z = '\033[1;31m'
X = '\033[1;33m'
Z1 = '\033[2;31m'
F = '\033[2;32m'
A = '\033[2;34m'
C = '\x1b[2;35m'
S = '\x1b[2;36m'
G = '\033[1;34m'
HH = '\033[1;34m'
red = "\033[1m\033[31m"
green = "\033[1m\033[32m"
yellow = "\033[1m\033[33m"
blue = "\033[1m\033[34m"
cyan = "\033[1m\033[36m"
magenta = "\033[1m\033[35m"
M = "\033[1m\033[36m"
white = "\033[1m\033[37m"
orange = "\033[1m\033[38;5;208m"
reset = "\033[0m"
O = '\x1b[38;5;208m'
Y = '\033[1;34m'
C = '\033[2;35m'
M = '\x1b[1;37m'
pink_t5ok5 = '\x1b[38;5;199m'
WHITE_BOLD = '\x1b[1;97m'
reset = '\x1b[0m'
import time
import random
import threading

# نولّد قائمة من 256 لون ANSI
colors_256 = [f"\033[38;5;{i}m" for i in range(16, 256)]

current_color = "\033[0m"

def color_changer():
    global current_color
    while True:
        current_color = random.choice(colors_256)
        time.sleep(0.1)

threading.Thread(target=color_changer, daemon=True).start()
saved_usernames = set()
saved_count = 0

def date(Id):
    try:
        Id = int(Id)
        if Id > 1545545 and Id < 1279000:
            return 2010
        elif Id > 1279001 and Id < 17750000:
            return 2011
        elif Id > 17750001 and Id < 279760000:
            return 2012
        elif Id > 279760001 and Id < 900990000:
            return 2013
        elif Id > 900990001 and Id < 1629010000:
            return 2014
        elif Id > 1900000000 and Id < 2500000000:
            return 2015
        elif Id > 2500000000 and Id < 3713668786:
            return 2016
        elif Id > 3713668786 and Id < 5699785217:
            return 2017
        elif Id > 5699785217 and Id < 8507940634:
            return 2018
        elif Id > 8507940634 and Id < 21254029834:
            return 2019
        else:
            return "2020-2023"
    except:
        return False

def search_and_save(target_years):
    global saved_count
    char_sets = [
        'azertyuiopmlkjhgfdsqwxcvbn', 'abcdefghijklmnopqrstuvwxyzéèêëàâäôùûüîïç',
        'abcdefghijklmnopqrstuvwxyzñ', 'абвгдеёжзийклмнопрстуфхцчшщъыьэюя',
        '的一是不了人我在有他这为之大来以个中上们到 说时国和地要就出会可也你对生能而子那得于着下自之',
        'アイウエオカキクケコサシスセソタチツテトナ ニヌネノハヒフヘホマミムメモヤユヨラリルレロワヲン',
        'あいうえおかきくけこさしすせそたちつてとな にぬねのはひふへほまみむめもやゆよらりるれろわをん',
        'אבגדהוזחטיכלמנסעפצקרשת', 'αβγδεζηθικλμνξοπρστυφχψω',
        'abcdefghijklmnopqrstuvwxyzç', 'กขฃคฅฆงจฉชซฌญฎฏฐฑฒณดตถทธนบปผฝพฟภมยรฤฤลฦวศษสหฬอฮ',
        'अआइईउऊऋएऐओऔअंअःकखगघङचछजझञटठडढणतथदधनपफबभमयरलवशषसहक्षत्रज्ञ'
    ]
    while True:
        try:
            g = choice(char_sets)
            keyword = ''.join((choice(g) for i in range(randrange(4, 9))))

            cookies = {
                'rur': '"LDC\\05467838469205\\0541758153066:01f72be7578ed09a57bfe3e41c19af58848e0e965e0549f6d1f5a0168a652d2bfa28cd9a"',
            }

            headers = {
                'accept': '*/*',
                'accept-language': 'ar,en-US;q=0.9,en;q=0.8',
                'content-type': 'application/x-www-form-urlencoded',
                'origin': 'https://www.instagram.com',
                'priority': 'u=1, i',
                'referer': 'https://www.instagram.com/',
                'sec-ch-prefers-color-scheme': 'light',
                'sec-ch-ua': '"Chromium";v="128", "Not;A=Brand";v="24", "Google Chrome";v="128"',
                'sec-ch-ua-full-version-list': '"Chromium";v="128.0.6613.138", "Not;A=Brand";v="24.0.0.0", "Google Chrome";v="128.0.6613.138"',
                'sec-ch-ua-mobile': '?0',
                'sec-ch-ua-model': '""',
                'sec-ch-ua-platform': '"Windows"',
                'sec-ch-ua-platform-version': '"15.0.0"',
                'sec-fetch-dest': 'empty',
                'sec-fetch-mode': 'cors',
                'sec-fetch-site': 'same-origin',
                'user-agent': generate_user_agent(),
                'x-asbd-id': '129477',
                'x-bloks-version-id': '235c9483d007713b45fc75b34c76332d68d579a4300a1db1da94670c3a05089f',
                'x-csrftoken': 'mf3zd6qWxnKgh9BaNRI5Ldpms2NrH62X',
                'x-fb-friendly-name': 'PolarisSearchBoxRefetchableQuery',
                'x-fb-lsd': 'BslibIYRWxn19hyIaPyrZV',
                'x-ig-app-id': '936619743392459',
            }

            data = {
                'variables': '{"data":{"context":"blended","include_reel":"true","query":"' + keyword + '","rank_token":"","search_surface":"web_top_search"},"hasQuery":true}',
                'doc_id': '7935512656557707',
            }

            response = requests.post('https://www.instagram.com/graphql/query', cookies=cookies, headers=headers, data=data).json()['data']['xdt_api__v1__fbsearch__topsearch_connection']['users']
            for Hus in response:
                d_7vw = Hus['user']['username']
                user_id = Hus['user']['id']
                creation_year = date(user_id)

                if str(creation_year) in target_years:
                    if d_7vw not in saved_usernames:
                        saved_usernames.add(d_7vw)
                        with open('user.txt', 'a', encoding='utf-8') as f:
                            f.write(d_7vw + '\n')
                        saved_count += 1
                        sys.stdout.write(f"\r{current_color}Saved: {saved_count} × User : {d_7vw}{mlham}    ")
                        sys.stdout.flush()
        except:
            continue

def start_searcher():
    os.system('cls' if os.name == 'nt' else 'clear')
    print(f"""
    """)
    try:
        choice = (f"10")
        target_years = []

        if choice == '1':
            target_years = ['2012']
        elif choice == '2':
            target_years = ['2013']
        elif choice == '3':
            target_years = ['2014']
        elif choice == '4':
            target_years = ['2015']
        elif choice == '5':
            target_years = ['2016']
        elif choice == '6':
            target_years = ['2017']
        elif choice == '7':
            target_years = ['2018']
        elif choice == '8':
            target_years = ['2019']
        elif choice == '9':
            target_years = ['2020-2023']
        elif choice == '10':
            target_years = ['2014', '2015', '2016', '2017', '2018', '2019', '2020-2023']
        elif choice == '11':
            target_years = ['2012', '2013']
        else:
            print(f"\n{E}خيار غير صالح. يرجى إعادة تشغيل البرنامج.{mlham}")
            sys.exit()

        time.sleep(0.5)

        with ThreadPoolExecutor(max_workers=300) as executor:
            for _ in range(300):
                executor.submit(search_and_save, target_years)
    except KeyboardInterrupt:
        print(f"\n\n{E}Search stopped. Total users saved: {saved_count}{mlham}")
        sys.exit()
    except Exception as e:
        print(f"\n{E}An unexpected error occurred: {e}{mlham}")
        sys.exit()

start_searcher()
