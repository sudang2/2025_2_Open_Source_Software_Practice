FROM ubuntu:latest

RUN apt-get update
RUN apt-get install -y python3

CMD ["python3", "-c", "\
def isHappy(n):\n\
    result=0\n\
    temp=n\n\
    list=[n]\n\
    while True:\n\
        for i in str(temp):\n\
            result+=(int(i))**2\n\
        if(result==1):\n\
            return True\n\
        else:\n\
            for i in list:\n\
                if(i==result):\n\
                    return False\n\
            list.append(result)\n\
            temp=result\n\
            result=0\n\
print(isHappy(19))\n\
print(isHappy(2))"]