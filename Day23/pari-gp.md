# [Pari/GP], 148 bytes

    a->c=concat;[p,q]=[c([[[i,j]|j<-[1..#a],a[i,j]==t]|i<-[1..#a~]])|t<-[1,2]];vecmin([#[1|y<-q,![u*v~>0|z<-c(p,q),!matdet(Mat([u=x-z,v=z-y]~))]]|x<-p])

[Try it online!][TIO-l0kmszvt]

[Pari/GP]: http://pari.math.u-bordeaux.fr/
[TIO-l0kmszvt]: https://tio.run/##bU5LasMwEL2Kk2ykMgpWtrJ8g55gmMWgJkGhcZWgmNgIX92V1Ba6CMOg99NjAt@9Oof11NiVVe@s@xocR4MBbmTRCUT0cKF06RTq/X7HBFwVayMl/6cuRDLFwuBAZMaju/pB4A51mjp1gw0@3salb9PcKSdyuYTNlePHMYp3jgIf9qlmGO2sJlqkJErPTgWSK4fwOQluVN@Eux9ihttCts1JsJTQYPmvM6g9GsoBRT5AHfP61ZQjbQHQmrx5tCksrykl2SuRX1jNtmJd4/9RdsxPVenNN38D "Pari/GP – Try It Online"