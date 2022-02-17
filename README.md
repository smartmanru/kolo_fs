gantt
    title A Gantt Diagram
    dateFormat  DD-MM-YYYY
    
    section фитнес сознания 0 offline
        поток 3 :active,fs0_3_offline, 10-02-2022,24-02-2022
    section фитнес сознания 1 offline
        поток 2  :done,fs1_2_offline,17-01-2022,14-02-2022
        поток 3  :crit,fs1_3_offline, 03-03-2022,05-05-2022
        %% поток 4  :fs1_4_offline,
        
    section фитнес сознания 2 offline
        поток 1  :done, fs2_1_offline, 09-12-2021,22-01-2022
        поток 2  :fs2_2_offline,
        %% поток 3  :fs2__offline,

    section фитнес сознания 3 offline
        поток 1  :done,fs3_1_offline,06-12-2021,12-01-2022 
        поток 2  :active,fs3_2_offline,14-02-2022,23-03-2022
        %% поток 3  :fs3_3_offline,

    section фитнес сознания 1 online
        поток 1  :done,fs1_1_online, 07-12-2021, 17-02-2022
        поток 2  :crit,fs1_2_online, after fs0_3_offline,10w
        %% поток 3  :fs1_3_online,

    section фитнес сознания 2 online
        поток 2 :crit,fs2_2_online, 22-02-2022,03-05-2022
        %% поток 3  :fs2_3_online,

    section фитнес сознания 3 online
        %% поток 1  :fs3_1_online, 
        %% поток 2  :fs3_2_online,
        %% поток 3  :fs3_3_online,
            
    
    section ВМ онлайн
        поток 1  :active,vm1_1_online, 24-01-2022,04-04-2022
    
    section ВМ оффлайн
        поток 1  :active,vm1_1_online,14-01-2022,29-03-2022 
        
    section Ретриты
        Путь к себе :crit,put_k_sebe, 05-03-2022,09-03-2022
