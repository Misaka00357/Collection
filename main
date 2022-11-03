#游戏
print('='*20,'舰队collection','='*20)
while True:
    print('='*56)
    print('请选择阵营：')
    print('\t1.舰娘')
    print('\t2.深海')
    choose=input('请选择【1/2】')
    print('='*56)
    if choose=='1':
        print('吹雪，出击！')
    elif choose=='2':
        print('不许投敌')
    else:
        print('选项不存在，镇守府将自动给你分配【吹雪】')
    #HP ATTACK
    plife=15
    patk=12
    pexp=0
    plvl=1
    blife=20
    batk=20
    print('='*56)
    print(f'吹雪：耐久={plife} 火力={patk}')#f字符串：格式化字符串
    while True:
        print('='*56)
        print('请选择操作：')
        print('\t1.演习')
        print('\t2.出击')
        print('\t3.撤退')
        choose=input('请选择【1/2/3】')
        if choose=='1':
            pexp+=3171
            plvl=int(0.5*(1+pow(1+0.08*pexp,0.5)))
            print('='*56)
            print(f'Level={plvl},exp={pexp}')
            while True:
                if plife>15:
                    break
                if plvl >=20:
                    a=input('是否改造？【Y/N】')
                    if a=='Y' or a=='y':
                        plife+=15
                        patk+=20
                        print('='*56)
                        print('[吹雪]变强了')
                break
        elif choose=='2':
            blife-=patk
            print('='*56)
            print(f'[吹雪]→[驱逐i级] {patk} damage')
            if blife<=0:
                print('='*56)
                print('[驱逐i级]被击沉了，战舰[大和]加入了游戏。游戏胜利')
                break
            plife-=batk
            print('='*56)
            print(f'[驱逐i级]→[吹雪] {batk} damage')
            if plife<=0:
                print('='*56)
                print('[吹雪]被击沉了，GAME OVER')
                break
        elif choose=='3':
            print('='*56)
            print('不许撤退')
        else:
            print('='*56)
            print('输入错误，请重新输入')
    rep=input('再玩一次【Y/N】')
    if rep!='Y' and rep!='y':
        break
    else:
        continue
