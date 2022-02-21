def frequencia(texto):
    
    dic = {}
    for nome in texto.split():
        if nome not in dic:
            dic[nome] = 0
        dic[nome] = dic[nome] + 1

    return sorted(sorted(dic), key=lambda x: dic[x], reverse = True)