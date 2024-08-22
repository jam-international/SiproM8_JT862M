// =========================================================
// SIPRO - M32
//
//  Definizione delle variabili CUCITRICE
//
// File DefCuci.h
// =========================================================


// ============================================================================
//      COSTANTI
// ============================================================================

// Definizioni canali contesti e matrici
// Il contesto del tabellone dei parametri dinamici e' definito in cucitrice.txt
#define     C1_PROFILO_CNTX     1       // [INT] Cucitrice 1 - contesto profilo udf di cucitura
#define     C2_PROFILO_CNTX     2       // [INT] Cucitrice 2 - contesto profilo udf di cucitura
#define     C1_PAR_CNTX         3       // [INT] Cucitrice 1 - contesto parametri ( C1_Param.udf )
#define     C2_PAR_CNTX         4       // [INT] Cucitrice 2 - contesto parametri ( C2_Param.udf )

#define     C1_PAR_BASE_MTX     101     // [INT] Matrice di base dei parametri ( C1_Param.udf )
#define     C1_TAB_BASE_MTX     102     // [INT] Matrice di base del tabellone dei parametri dinamici
#define     C1_PROF_BASE_MTX    111     // [INT] Matrice di base del profilo udf di cucitura
#define     C1_PROF_HDR_MTX     112     // [INT] Matrice di header del profilo udf di cucitura

#define     C2_PAR_BASE_MTX     201     // [INT] Matrice di base dei parametri ( C2_Param.udf )
#define     C2_TAB_BASE_MTX     202     // [INT] Matrice di base del tabellone dei parametri dinamici
#define     C2_PROF_BASE_MTX    211     // [INT] Matrice di base del profilo udf di cucitura
#define     C2_PROF_HDR_MTX     212     // [INT] Matrice di header del profilo udf di cucitura


// Parametro CuciMode dell'istruzione ISO G281

#define     CA_MD_NO_MOVE       1       // Non attiva il movimento della cucitrice
#define     CA_MD_NO_RESET      2       // Non azzera il buffer
#define     CA_MD_NO_EXT_REWIND 4       // Non riporta all'inizio l'indice di estrazione
#define     CA_MD_NO_INS_PNT    8       // Non inserisce strutture punti
#define     CA_MD_NO_INS_G0     16      // Non inserisce movimenti di tipo G0
#define     CA_MD_NO_FIRST_J    64      // Non si parte dal primo punto (modello J)

#define     CA_MD_NO_RES_NO_INS         10  // CA_MD_NO_RESET+CA_MD_NO_INS_PNT
#define     CA_MD_NO_RES_NO_INS_NO_REW 126  // CA_MD_NO_RESET+CA_MD_NO_INS_PNT+CA_MD_NO_EXT_REWIND+CA_MD_NO_FIRST_J


// ============================================================================
//      ASSEGNAZIONE VB
// ============================================================================

//------------------------------------------------------------------------
// Vb1 - Vb1000 Variabili di uso generale
//
// definizioni in DefVar.h
//------------------------------------------------------------------------

//------------------------------------------------------------------------
// Vb1001 - Vb1950 Variabili per la cucitrice 1

#define C1_VbEnableCamme        vb1001      // Comando di abilitazione camme della cucitrice 1
#define C1_CmdInitCamme         vb1002      // Comando di inizializzazione delle camme digitali
#define C1_CmdPiedinoSu         vb1003      // Comando per alzare il piedino
#define C1_CmdPiedinoGiu        vb1004      // Comando per abbassare il piedino
#define C1_CmdRiposiziona       vb1005      // Comando di riposizionamento sul punto di cucitura
#define C1_CmdSimulaAva         vb1006      // Comando di Simula avanti
#define C1_CmdSimulaInd         vb1007      // Comando di Simula indietro
#define C1_CmdReloadTabellone   vb1008      // Comando di reload tabellone
#define C1_CmdHoldRelease       vb1009      // Comando interno di Hold/Release
#define C1_CmdHoldHMI           vb1010      // Comando Hold da HMI
#define C1_CmdReleaseHMI        vb1011      // Comando Release da HMI
#define C1_CmdSaveParam         vb1012      // Comando di save parametri
#define C1_CmdGantryCrochet     vb1013      // Comando di aggancio inseguimento gantry crochet
#define C1_CmdStdFollowCrochet  vb1014      // Comando di aggancio inseguimento standard crochet
#define C1_CmdSganciaCrochet    vb1015      // Comando di sgancio  inseguimento crochet
#define C1_CmdSetOffsetAgoTacca vb1016      // Comando di set offset ago - tacca di zero
#define C1_CmdGetOffsetAgoTacca vb1017      // Comando di acquisizione offset ago - tacca di zero
#define C1_CmdSbloccaAgo        vb1018      // Comando di sblocco dell'ago per movimento "a mano"
#define C1_CmdForceLoadProfilo  vb1019      // Comando di forzatura load profilo

#define C1_CmdSimulaAvaNpoint   vb1020      // Comando di Simula avanti n-punti
#define C1_CmdSimulaIndNpoint   vb1021      // Comando di Simula indietro n-punti

#define C1_SIMULA_AVA_CONT_IDX  1022        // [INT]
#define C1_SIMULA_IND_CONT_IDX  1023        // [INT]
#define C1_CmdSimulaAvaCont     vb1022      // Comando di Simula avanti n-punti
#define C1_CmdSimulaIndCont     vb1023      // Comando di Simula indietro n-punti

#define C1_CmdLoadParam         vb1024      // Comando di load del file UDF dei parametri
#define C1_ReloadParam          vb1025      // Forza il ricalcolo dei parametri

#define C1_ModoSimulaNpoint     vb1026      // Modo di Simulazione n-punti (0=tutti i punti  1=ultimo punto)

#define C1_CmdSimulaPedaleVel   vb1027      // Pedale per alta velocita' simulazione continua
#define C1_CuciBufRewind        vb1028      // Comando Rewind nella ripartenza


#define C1_AGO_FUORI_ING_IDX    1030        // [INT]
#define C1_AgoFuoriIngombro     vb1030      // Flag segnalazione asse in camma fuori ingombro

#define C1_AsseAgoFermo         vb1031      // Flag segnalazione asse ago fermo
#define C1_AssiAzzerati         vb1032      // Flag segnalazione assi azzerati

#define C1_FLG_CUCI_OR_MOVE_IDX 1033        // [INT]
#define C1_VbFlgCuciOrMove      vb1033      // Flag FlgCuciOrMove ( 1=cuci  0=move )

#define C1_CuciSimulaAuto       vb1034      // Esecuzione cucitura simulata per il CNC
#define C1_CuciLastPoint        vb1035      // Esecuzione ultimo punto di cucitura
#define C1_CuciLastPointEnaStop vb1036      // Consenso stop su ago alto ( last point )

#define C1_AGO_ALTO_STOP_IDX    1037        // [INT]
#define C1_CammaStopAgoAlto     vb1037      // Camma per stop ago alto

#define C1_FLG_G280_RUNNING_IDX 1038        // [INT]
#define C1_VbFlgG280Running     vb1038      // Flag FlgG280Running

#define C1_VbEnableCammeIni     vb1039      // Comando di abilitazione camme della cucitrice 1 start asse
#define C1_CuciLastPointAxC     vb1040      // Last point: gestione hold asse C

#define C1_FLG_JTASK_INFO_IDX   1041        // [INT]
#define C1_VbFlgJtaskRunning    vb1041      // Flag JTask running
#define C1_VbFlgJtaskLoopHold   vb1042      // Flag JTask loop hold
#define C1_FinitoSimulazione    vb1043      // il comando Simula è arrivato all'ultimo punto



    // Variabili a bit status word cucitrice
#define C1_STATUS_WORD_BIT_IDX  1850        // [INT] STATUS_WORD_BIT_IDX
#define C1_VbStEnIrqBit         vb1850      // Stato abilitazione IRQ
#define C1_VbStEnMovBit         vb1851      // Stato abilitazione movimento cucitura
#define C1_VbStDisAlarmBit      vb1852      // Stato generazione allarme ( 1=disab 0=enab )
#define C1_VbStAlarmBit         vb1853      // Stato allarme cucitrice
#define C1_VbStIrqBit           vb1854      // Stato IRQ cucitrice
#define C1_VbStCamMovBit        vb1855      // Stato camma movimento
#define C1_VbStSelEnc0Bit       vb1856      // Stato bit 0 selezione encoder
#define C1_VbStSelEnc1Bit       vb1857      // Stato bit 1 selezione encoder
#define C1_VbStAxMovBit         vb1858      // Stato asse in movimento
#define C1_VbStBit9             vb1859      // Stato bit 9
#define C1_VbStBit10            vb1860      // Stato bit 10
#define C1_VbStBit11            vb1861      // Stato bit 11
#define C1_VbStBit12            vb1862      // Stato bit 12
#define C1_VbStBit13            vb1863      // Stato bit 13
#define C1_VbStBit14            vb1864      // Stato bit 14
#define C1_VbStBit15            vb1865      // Stato bit 15

//------------------------------------------------------------------------
// Vb1951 - Vb1999 Variabili di interfaccia con firmware Cucitrice e PLC
// ( c:\cnc\sys\cucitrice.txt )

#define C1_VbStartCuci          vb1951
#define C1_VbHoldCuci           vb1952
#define C1_VbReleaseCuci        vb1953
#define C1_VbEndCuci            vb1954
#define C1_VbRunCuci            vb1955
#define C1_VbRallCuci           vb1956
#define C1_VbRasafCuci          vb1957
#define C1_VbAgoAzzCuci         vb1958
#define C1_VbCamMovCuci         vb1959
#define C1_VbAxMovCuci          vb1960
#define C1_VbLastPnt            vb1961
#define C1_VbSuspendCuci        vb1962
#define C1_VbCuciIsoActive      vb1963
#define C1_VbCuciGoto           vb1964

//------------------------------------------------------------------------
// Vb2001 - Vb2950 Variabili per la cucitrice 2

#define C2_VbEnableCamme        vb2001      // Comando di abilitazione camme della cucitrice 2
#define C2_CmdInitCamme         vb2002      // Comando di inizializzazione delle camme digitali
#define C2_CmdPiedinoSu         vb2003      // Comando per alzare il piedino
#define C2_CmdPiedinoGiu        vb2004      // Comando per abbassare il piedino
#define C2_CmdRiposiziona       vb2005      // Comando di riposizionamento sul punto di cucitura
#define C2_CmdSimulaAva         vb2006      // Comando di Simula avanti
#define C2_CmdSimulaInd         vb2007      // Comando di Simula indietro
#define C2_CmdReloadTabellone   vb2008      // Comando di reload tabellone
#define C2_CmdHoldRelease       vb2009      // Comando interno di Hold/Release
#define C2_CmdHoldHMI           vb2010      // Comando Hold da HMI
#define C2_CmdReleaseHMI        vb2011      // Comando Release da HMI
#define C2_CmdSaveParam         vb2012      // Comando di save parametri
#define C2_CmdGantryCrochet     vb2013      // Comando di aggancio inseguimento gantry crochet
#define C2_CmdStdFollowCrochet  vb2014      // Comando di aggancio inseguimento standard crochet
#define C2_CmdSganciaCrochet    vb2015      // Comando di sgancio  inseguimento crochet
#define C2_CmdSetOffsetAgoTacca vb2016      // Comando di set offset ago - tacca di zero
#define C2_CmdGetOffsetAgoTacca vb2017      // Comando di acquisizione offset ago - tacca di zero
#define C2_CmdSbloccaAgo        vb2018      // Comando di sblocco dell'ago per movimento "a mano"
#define C2_CmdForceLoadProfilo  vb2019      // Comando di forzatura load profilo

#define C2_CmdSimulaAvaNpoint   vb2020      // Comando di Simula avanti n-punti
#define C2_CmdSimulaIndNpoint   vb2021      // Comando di Simula indietro n-punti

#define C2_SIMULA_AVA_CONT_IDX  2022        // [INT]
#define C2_SIMULA_IND_CONT_IDX  2023        // [INT]
#define C2_CmdSimulaAvaCont     vb2022      // Comando di Simula avanti n-punti
#define C2_CmdSimulaIndCont     vb2023      // Comando di Simula indietro n-punti

#define C2_CmdLoadParam         vb2024      // Comando di load del file UDF dei parametri
#define C2_ReloadParam          vb2025      // Forza il ricalcolo dei parametri

#define C2_ModoSimulaNpoint     vb2026      // Modo di Simulazione n-punti (0=tutti i punti  1=ultimo punto)

#define C2_CmdSimulaPedaleVel   vb2027      // Pedale per alta velocita' simulazione continua
#define C2_CuciBufRewind        vb2028      // Comando Rewind nella ripartenza


#define C2_AGO_FUORI_ING_IDX    2030        // [INT]
#define C2_AgoFuoriIngombro     vb2030      // Flag segnalazione asse in camma fuori ingombro

#define C2_AsseAgoFermo         vb2031      // Flag segnalazione asse ago fermo
#define C2_AssiAzzerati         vb2032      // Flag segnalazione assi azzerati

#define C2_FLG_CUCI_OR_MOVE_IDX 2033        // [INT]
#define C2_VbFlgCuciOrMove      vb2033      // Flag FlgCuciOrMove ( 1=cuci  0=move )

#define C2_CuciSimulaAuto       vb2034      // Esecuzione cucitura simulata per il CNC
#define C2_CuciLastPoint        vb2035      // Esecuzione ultimo punto di cucitura
#define C2_CuciLastPointEnaStop vb2036      // Consenso stop su ago alto ( last point )

#define C2_AGO_ALTO_STOP_IDX    2037        // [INT]
#define C2_CammaStopAgoAlto     vb2037      // Camma per stop ago alto

#define C2_FLG_G280_RUNNING_IDX 2038        // [INT]
#define C2_VbFlgG280Running     vb2038      // Flag FlgG280Running

#define C2_VbEnableCammeIni     vb2039      // Comando di abilitazione camme della cucitrice 2 start asse
#define C2_CuciLastPointAxC     vb2040      // Last point: gestione hold asse C

#define C2_FLG_JTASK_INFO_IDX   2041        // [INT]
#define C2_VbFlgJtaskRunning    vb2041      // Flag JTask running
#define C2_VbFlgJtaskLoopHold   vb2042      // Flag JTask loop hold
#define C2_FinitoSimulazione    vb2043      // il comando Simula è arrivato all'ultimo punto


    // Variabili a bit status word cucitrice
#define C2_STATUS_WORD_BIT_IDX  2850        // [INT] STATUS_WORD_BIT_IDX
#define C2_VbStEnIrqBit         vb2850      // Stato abilitazione IRQ
#define C2_VbStEnMovBit         vb2851      // Stato abilitazione movimento cucitura
#define C2_VbStDisAlarmBit      vb2852      // Stato generazione allarme ( 1=disab 0=enab )
#define C2_VbStAlarmBit         vb2853      // Stato allarme cucitrice
#define C2_VbStIrqBit           vb2854      // Stato IRQ cucitrice
#define C2_VbStCamMovBit        vb2855      // Stato camma movimento
#define C2_VbStSelEnc0Bit       vb2856      // Stato bit 0 selezione encoder
#define C2_VbStSelEnc1Bit       vb2857      // Stato bit 1 selezione encoder
#define C2_VbStAxMovBit         vb2858      // Stato asse in movimento
#define C2_VbStBit9             vb2859      // Stato bit 9
#define C2_VbStBit10            vb2860      // Stato bit 10
#define C2_VbStBit11            vb2861      // Stato bit 11
#define C2_VbStBit12            vb2862      // Stato bit 12
#define C2_VbStBit13            vb2863      // Stato bit 13
#define C2_VbStBit14            vb2864      // Stato bit 14
#define C2_VbStBit15            vb2865      // Stato bit 15

//------------------------------------------------------------------------
// Vb2951 - Vb2999 Variabili di interfaccia con firmware Cucitrice e PLC
// ( c:\cnc\sys\cucitrice.txt )

#define C2_VbStartCuci          vb2951
#define C2_VbHoldCuci           vb2952
#define C2_VbReleaseCuci        vb2953
#define C2_VbEndCuci            vb2954
#define C2_VbRunCuci            vb2955
#define C2_VbRallCuci           vb2956
#define C2_VbRasafCuci          vb2957
#define C2_VbAgoAzzCuci         vb2958
#define C2_VbCamMovCuci         vb2959
#define C2_VbAxMovCuci          vb2960
#define C2_VbLastPnt            vb2961
#define C2_VbSuspendCuci        vb2962
#define C2_VbCuciIsoActive      vb2963
#define C2_VbCuciGoto           vb2964

//------------------------------------------------------------------------
// Vb3000 - Vb7000 Variabili di uso generale
//
// definizioni in DefVar.h
//------------------------------------------------------------------------




// ============================================================================
//      ASSEGNAZIONE VN
// ============================================================================

//------------------------------------------------------------------------
// Vn1 - Vn1000 Variabili di uso generale
//
// definizioni in DefVar.h
//------------------------------------------------------------------------

//------------------------------------------------------------------------
// Vn1001 - Vn1900 Variabili per la cucitrice 1

    // contesto cucitrice
#define C1_TAB_CONTEXT_IDX      1001        // [INT]
#define C1_TabParContext        vn1001      // Contesto pr UDF cucitrice
#define C1_VelLavRPM            vn1002      // Velocita' di lavoro ( per FunPlc )
#define C1_VelLimitRPM          vn1003      // Limitazione RPM Ago
#define C1_PlcStatoAgo          vn1004      // Stato Ago ( macchina a stati PLC )
#define C1_PlcStatoScartafilo   vn1005      // Stato scartafilo  ( macchina a stati PLC )
#define C1_MovAxCStatus         vn1006      // Stato asse C ( macchina a stati PLC )

#define C1_RD_NEXT_CODE_IDX     1010        // [INT]
#define C1_NextCode             vn1010      // Codice prossimo movimento simulato ( fun 281 cmd 48 e 49 )
#define C1_WRITE_PAR_IDX        1011        // [INT]
#define C1_StepNum              vn1011      // Numero del passo da scrivere
#define C1_MtxNum               vn1012      // Numero della matrice di base

#define mc_stati_C1CmdSimula        vn1020  //indice macchina stati per gestione piedino durante simula
#define mc_stati_C1CmdSimulaCont    vn1021  //indice macchina stati per gestione piedino durante simula continuo


    // Interfaccia per lettura e scrittura parametri azionamento Delta ASDA-A2
#define C1_SDO_ERRCODE_IDX      1680        // [INT] Servizio SDO - ErrorCode
#define C1_SDO_ErrCode          vn1680      // Error Code

#define C1_SDO_RW_PAR_IDX       1681        // [INT] Servizio SDO - Parametri
#define C1_SDO_Network          vn1681      // Rete
#define C1_SDO_Node             vn1682      // Nodo
#define C1_SDO_ObjIndex         vn1683      // Index
#define C1_SDO_SubIndex         vn1684      // SubIndex
#define C1_SDO_Size             vn1685      // Size
#define C1_SDO_VqDataIdx        vn1686      // Vq data index

#define C1_SetParamStatus       vn1690      // Status
#define C1_SetParamErrCode      vn1691      // ErrorCode
#define C1_SetParamCmd          vn1692      // Cmd  1=rd  2=wr

#define C1_SetParamAxNum        vn1693      // Axis Number [1,2,...]
#define C1_SetParamCat          vn1694      // Categoria di parametri
#define C1_SetParamIdx          vn1695      // Indice del parametro
#define C1_SetParamSize         vn1696      // Size del parametro [ 1=byte  2=word  4=long ]

//------------------------------------------------------------------------
// Vn1901 - Vn1950 Profilo di cucitura UDF - Variabili matrici base e header
// Matrice di base   Id=111
// Matrice di header Id=112

#define C1_BaseOpCode           vn1901      // Op code ( matrice di base )

//------------------------------------------------------------------------
// Vn1951 - Vn1999 Variabili di interfaccia con firmware Cucitrice e PLC
// ( c:\cnc\sys\cucitrice.txt )

#define C1_VN_STATUS_CUCI_IDX   1952        // [INT] Status cucitrice

#define C1_VnErrCuci            vn1951      // Error code
#define C1_VnStatusCuci         vn1952      // Vn status
#define C1_VnZeroCuci           vn1953      // Contatore tacche di zero
#define C1_VnPntRallCuci        vn1954      // Punti di rallentamento
#define C1_VnOvdAxAgo           vn1955      // Override asse ago
#define C1_VnRpmMaxAgo          vn1956      // Vel max ago
#define C1_VnInfoPoint          vn1957      // Info point

//------------------------------------------------------------------------
// Vn2001 - Vn2900 Variabili per la cucitrice 2

    // contesto cucitrice
#define C2_TAB_CONTEXT_IDX      2001        // [INT]
#define C2_TabParContext        vn2001      // Contesto pr UDF cucitrice
#define C2_VelLavRPM            vn2002      // Velocita' di lavoro ( per FunPlc )
#define C2_VelLimitRPM          vn2003      // Limitazione RPM Ago
#define C2_PlcStatoAgo          vn2004      // Stato Ago ( macchina a stati PLC )
#define C2_PlcStatoScartafilo   vn2005      // Stato scartafilo  ( macchina a stati PLC )
#define C2_MovAxCStatus         vn2006      // Stato asse C ( macchina a stati PLC )

#define C2_RD_NEXT_CODE_IDX     2010        // [INT]
#define C2_NextCode             vn2010      //  Codice prossimo movimento simulato ( fun 281 cmd 48 e 49 )
#define C2_WRITE_PAR_IDX        2011        // [INT]
#define C2_StepNum              vn2011      // Numero del passo da scrivere
#define C2_MtxNum               vn2012      // Numero della matrice di base


#define mc_stati_C2CmdSimula        vn2020
#define mc_stati_C2CmdSimulaCont    vn2021
//------------------------------------------------------------------------
// Vn2901 - Vn2950 Profilo di cucitura UDF - Variabili matrici base e header
// Matrice di base   Id=211
// Matrice di header Id=212

#define C2_BaseOpCode           vn2901      // Op code ( matrice di base )

//------------------------------------------------------------------------
// Vn1952 - Vn2999 Variabili di interfaccia con firmware Cucitrice e PLC
// ( c:\cnc\sys\cucitrice.txt )

#define C2_VN_STATUS_CUCI_IDX   2952        // [INT] Status cucitrice

#define C2_VnErrCuci            vn2951      // Error code
#define C2_VnStatusCuci         vn2952      // Vn status
#define C2_VnZeroCuci           vn2953      // Contatore tacche di zero
#define C2_VnPntRallCuci        vn2954      // Punti di rallentamento
#define C2_VnOvdAxAgo           vn2955      // Override asse ago
#define C2_VnRpmMaxAgo          vn2956      // Vel max ago
#define C2_VnInfoPoint          vn2957      // Info point



// ============================================================================
//      ASSEGNAZIONE VQ
// ============================================================================

//------------------------------------------------------------------------
// Vq1 - Vq1000 Variabili di uso generale
//
// definizioni in DefVar.h
//------------------------------------------------------------------------

//------------------------------------------------------------------------
// Vq1001 - Vq1700 Variabili per la cucitrice 1

#define C1_VEL_RIF_AGO          1001
#define C1_VelRifAgo            vq1001      // Velocita' riferimento asse ago

#define C1_IMP_RIF_AGO          1002
#define C1_ImpRifAgo            vq1002      // Impulsi riferimento asse ago

#define C1_MM_RIF_AGO           1003
#define C1_MmRifAgo             vq1003      // Mm riferimento asse ago

#define C1_PT_INI_IDX           1004
#define C1_PtIni                vq1004      // Punti iniziali
#define C1_RpmIni               vq1005      // RPM punti iniziali

#define C1_PT_RALL_IDX          1006
#define C1_PtRall               vq1006      // Punti finali
#define C1_RpmRall              vq1007      // RPM punti finali

#define C1_VelMaxAgoRPM         vq1008      // Vel max RPM AGO

#define C1_CntApritens          vq1009      // Contatore impulsi uscita apritensione
#define C1_CntColtello          vq1010      // Contatore impulsi uscita coltello

#define C1_SIMULA_NPOINT_IDX    1011        // [INT]
#define C1_SimulaNumPoint       vq1011      // Numero di punti simulazione
#define C1_SimulaNumPointVel    vq1012      // Vel [%] simulazione npoint
#define C1_SimulaNumPointMsk    vq1013      // Maschera simulazione npoint

#define C1_SIMULA_CONT_IDX      1015        // [INT]
#define C1_SimulaContVbIdx      vq1015      // Indice Vb
#define C1_SimulaContVel1       vq1016      // Vel [%] simulazione continua
#define C1_SimulaContVel2       vq1017      // Vel [%] simulazione continua
#define C1_SimulaContVel3       vq1018      // Vel [%] simulazione continua
#define C1_SimulaContPt12       vq1019      // N. punti cambio da Vel1 a Vel2
#define C1_SimulaContPt23       vq1020      // N. punti cambio da Vel2 a Vel3
#define C1_SimulaContVbPedale   vq1021      // Indice VB pedale per alta velocita'
#define C1_SimulaContVelPedale  vq1022      // Vel pedale alta velocita'[%] simulazione continua

#define C1_FIRST_PT_IDX         1025        // [INT]
#define C1_FirstPtContext       vq1025      // Contesto UDF per calcolo primo punto
#define C1_FirstPtValid         vq1026      // Flag primo punto valido
#define C1_FirstPt_X            vq1027      // Coordinata X del primo punto
#define C1_FirstPt_Y            vq1028      // Coordinata Y del primo punto
#define C1_FirstPt_C            vq1029      // Coordinata C iniziale

#define C1_GANTRY_INFO_IDX      1030        // [INT]
#define C1_GantryErrAct         vq1030      // Errore istantaneo
#define C1_GantryErrMax         vq1031      // Errore massimo
#define C1_GantryErrReset       vq1032      // Reset errore massimo

#define C1_CALC_BUF_IDX         1035        // [INT]
#define C1_CalcBufContext       vq1035      // Contesto ( dato di input )
#define C1_CalcBufErrCode       vq1036      // Codice di errore
#define C1_CalcBufErrStepNum    vq1037      // N. passo UDF dove e' avventuto l'errore
#define C1_CalcBufErrPar        vq1038      // Parametro aggiuntivo dell'errore

#define C1_WARNING_INFO_IDX     1040        // [INT]
#define C1_WarningFlg           vq1040      // Flag Warning
#define C1_WarningAntXMm        vq1041      // Mm per il calcolo dell'anticipo  X
#define C1_WarningAntXRpm       vq1042      // RPM per il calcolo dell'anticipo X
#define C1_WarningAntXPassoUdf  vq1043      // Passo UDF per il calcolo dell'anticipo X
#define C1_WarningAntYMm        vq1044      // Mm per il calcolo dell'anticipo  Y
#define C1_WarningAntYRpm       vq1045      // RPM per il calcolo dell'anticipo Y
#define C1_WarningAntYPassoUdf  vq1046      // Passo UDF per il calcolo dell'anticipo Y
#define C1_WarningFreqXMm       vq1047      // Mm per il calcolo delle frequenze X
#define C1_WarningFreqXRpm      vq1048      // RPM per il calcolo delle frequenze X
#define C1_WarningFreqXPassoUdf vq1049      // Passo UDF per il calcolo delle frequenze X
#define C1_WarningFreqYMm       vq1050      // Mm per il calcolo delle frequenze Y
#define C1_WarningFreqYRpm      vq1051      // RPM per il calcolo delle frequenze Y
#define C1_WarningFreqYPassoUdf vq1052      // Passo UDF per il calcolo delle frequenze Y
#define C1_CntBloccoFiloINI     vq1053      // Contatore impulsi uscita BloccoFiloINI
#define C1_CntBloccoFiloEND     vq1054      // Contatore impulsi uscita BloccoFiloEND


#define C1_FUN74_IDX            1060        // [INT]
#define C1_Fun74_RetCode        vq1060      // RetCode
#define C1_Fun74_QuoObj         vq1061      // Quota obiettivo
#define C1_Fun74_VelObj         vq1062      // Velocita'
#define C1_Fun74_Future         vq1063      // Future
#define C1_Fun74_Acc            vq1063      // Accelerazione ( polinomio grado 5 )
#define C1_Fun74_Tmov           vq1064      // Tempo di movimento ( polinomio grado 5 )
#define C1_Fun74_Offs           vq1065      // Offset anticipo start ( polinomio grado 5 )

#define C1_FASE_AX_AGO_IDX      1070        // [INT]
#define C1_FaseAxAgo            vq1070      // Fase asse ago

#define C1_FASE_AX_C_IDX        1071        // [INT]
#define C1_FaseAxC              vq1071      // Fase asse C

#define C1_CMD_QUO_ABS_IDX      1075        // [INT]
#define C1_CmdQuoAbsRet         vq1075      // RetCode
#define C1_CmdQuoAbsX           vq1076      // QuoAbs X
#define C1_CmdQuoAbsY           vq1077      // QuoAbs Y
#define C1_CmdQuoAbsC           vq1078      // QuoAbs C

#define C1_RPM_AGO_PROFILO_IDX  1100        // [INT]
#define C1_RpmAgoInProfilo      vq1100      // Rpm ago impostati da istruzione del profile ( Vcd1 )

#define C1_TENSIONE_PROFILO_IDX 1101        // [INT]
#define C1_TensioneInProfilo    vq1101      // tensione impostata da istruzione del profile ( Vcd2 )

#define C1_VelRiduzioneRPM      vq1110      // Ulteriore limite RPM Ago ( #M200710_1GF# )

#define C1_CMD_MOVE_AX_C_IDX    1120        // [INT]
#define C1_CmdMoveAxC           vq1120      // Comando di movimento asse C
#define C1_QuoObjAxC            vq1121      // Quota obiettivo asse C
#define C1_NumPtMoveAxC         vq1122      // Punti di cucitura - movimento asse C
#define C1_RpmMoveAxC           vq1123      // Rpm ago durante il movimento dell'asse C
#define C1_IrqNumMoveAxC        vq1124      // IrqNumber interpretazione movimento dell'asse C

#define C1_CMD_GET_IRQ_CNT_IDX  1127        // [INT]
#define C1_IrqCnt               vq1127      // Contatore Irq ( Fun 281 cmd 63 )

#define C1_MOVE_PLC_AX_C_IDX    1130        // [INT]
#define C1_MovePlcAxCErrCode    vq1130      // Mov. asse C - ErrorCode
#define C1_MovePlcAxCQuoObj     vq1131      // Mov. asse C - Quota obiettivo
#define C1_MovePlcAxCVel        vq1132      // Mov. asse C - Velocita'
#define C1_MovePlcAxCAcc        vq1133      // Mov. asse C - Accelerazione
#define C1_MovePlcAxCTime       vq1134      // Mov. asse C - Tempo di movimento
#define C1_MovePlcAxCAnt        vq1135      // Mov. asse C - Anticipo

//------------------------------------------------------------------------
// Vq1651 - Vq1700 Informazioni di debugger del tabellone dei parametri
#define C1_InfoCntPunti         vq1651      // Contatore punti di cucitura
#define C1_InfoAnticipoMm       vq1652      // Mm per il calcolo dell'anticipo
#define C1_InfoAnticipoRpm      vq1653      // RPM per il calcolo dell'anticipo
#define C1_InfoAnticipoPassoUdf vq1654      // Passo UDF per il calcolo dell'anticipo
#define C1_InfoFreqXMm          vq1655      // Mm per il calcolo delle frequenze X
#define C1_InfoFreqXRpm         vq1656      // RPM per il calcolo delle frequenze X
#define C1_InfoFreqXPassoUdf    vq1657      // Passo UDF per il calcolo delle frequenze X
#define C1_InfoFreqYMm          vq1658      // Mm per il calcolo delle frequenze Y
#define C1_InfoFreqYRpm         vq1659      // RPM per il calcolo delle frequenze Y
#define C1_InfoFreqYPassoUdf    vq1660      // Passo UDF per il calcolo delle frequenze Y

    // Interfaccia per lettura e scrittura parametri azionamento Delta ASDA-A2
#define C1_SDO_VQ_DATA_IDX      1690        // [INT] Servizio SDO - Vq dato letto o da scrivere
#define C1_SDO_VqRwData         vq1690      // Vq dato letto o da scrivere

//------------------------------------------------------------------------
// Vq1701 - Vq1850 Parametri cucitrice  - Variabili matrici base
// Matrice di base   Id=101

#define C1_SGL_START_STOP_IDX   1701        // [INT]
#define C1_OFFSET_AGO_TACCA_IDX 1716        // [INT]

#define C1_SogliaStart          vq1701      // Soglia start movimento [gradi]
#define C1_SogliaStop           vq1702      // Soglia stop  movimento [gradi]
#define C1_AgoAlto              vq1703      // Ago alto [gradi]
#define C1_StartApriTens        vq1704      // Start camma apritensione [gradi]
#define C1_StopApriTens         vq1705      // Stop  camma apritensione [gradi]
#define C1_StartColtello        vq1706      // Start camma coltello [gradi]
#define C1_StopColtello         vq1707      // Stop  camma coltello [gradi]
#define C1_TSalitaPiedino       vq1708      // Tempo salita piedino [s]
#define C1_TDiscesaPiedino      vq1709      // Tempo discesa piedino [s]
#define C1_ParVelLavRPM         vq1710      // Vel. lavoro ago [RPM]
#define C1_ParPuntiVelIni       vq1711      // Punti iniziali (no fix3)
#define C1_ParVelIniRPM         vq1712      // Vel iniziale ago [RPM]
#define C1_ParPuntiVelRall      vq1713      // Punti rallentamento (no fix3)
#define C1_ParVelRallRPM        vq1714      // Vel rallentamento ago [RPM]
#define C1_StopAgo              vq1715      // Quota stop dell'ago (prima del movimento ad ago alto)
#define C1_OffsetAgoTacca       vq1716      // Offset di fase tran la quota dell'ago e la tacca di zero
#define C1_Par_FeedG0Reset      vq1717      // Feed nei movimenti G0 per azzeramento o reset [mm/min] fix3
#define C1_StartBloccoFiloINI   vq1718      // Start camma blocco filo inizio cucitura [gradi]
#define C1_StopBloccoFiloINI    vq1719      // Stop camma blocco filo inizio cucitura [gradi]
#define C1_StartBloccoFiloEND   vq1720      // Start camma blocco filo fine cucitura [gradi]
#define C1_StopBloccoFiloEND    vq1721      // Stop camma blocco filo fine cucitura [gradi]
#define C1_ParVelRotazione      vq1722      // Velocita' asse C rotazione [%] fix3 movimento iniziale
#define C1_Par_23               vq1723
#define C1_Par_24               vq1724
#define C1_Par_25               vq1725
#define C1_Par_26               vq1726
#define C1_Par_27               vq1727
#define C1_Par_28               vq1728
#define C1_Par_29               vq1729
#define C1_Par_30               vq1730
#define C1_Par_31               vq1731
#define C1_Par_32               vq1732
#define C1_Par_33               vq1733
#define C1_Par_34               vq1734
#define C1_Par_35               vq1735
#define C1_Par_36               vq1736
#define C1_Par_37               vq1737
#define C1_Par_38               vq1738
#define C1_Par_39               vq1739
#define C1_Par_40               vq1740

// Le variabili seguenti servono per origini, rototraslazioni e fattori di scala
//#define C1_ScaleFactX           vq1821      // Fattore di scala X
//#define C1_ScaleFactY           vq1822      // Fattore di scala Y
//#define C1_ScaleCenterX         vq1823      // Centro di scalatura X
//#define C1_ScaleCenterY         vq1824      // Centro di scalatura Y

//#define C1_RotCenterX           vq1825      // Centro di rotazione X
//#define C1_RotCenterY           vq1826      // Centro di rotazione Y
//#define C1_Rotation             vq1827      // Angolo di rotazione

//#define C1_OriginX              vq1828      // Origine X
//#define C1_OriginY              vq1829      // Origine Y
//------------------

// Le variabili seguenti non servono se si usa il tabellone dei parametri dinamici
// Se non si usa il tabellone, queste variabili vanno inserite nella matrice dei parametri
//@// #define C1_ACC_DEC_X_IDX        1830
//@// #define C1_StepAccX             vq1830      // Step accelerazione asse X [step]
//@// #define C1_StepDecX             vq1831      // Step decelerazione asse X [step]

//@// #define C1_FREQ_X_IDX           1832
//@// #define C1_FreqAccX             vq1832      // Freq. accelerazione asse X [KHz]
//@// #define C1_FreqLavX             vq1833      // Freq. lavoro asse X [KHz]
//@// #define C1_FreqDecX             vq1834      // Freq. decelerazione asse X [KHz]

//@// #define C1_ACC_DEC_Y_IDX        1840
//@// #define C1_StepAccY             vq1840      // Step accelerazione asse Y [step]
//@// #define C1_StepDecY             vq1841      // Step decelerazione asse Y [step]

//@// #define C1_FREQ_Y_IDX           1842
//@// #define C1_FreqAccY             vq1842      // Freq. accelerazione asse Y [KHz]
//@// #define C1_FreqLavY             vq1843      // Freq. lavoro asse Y [KHz]
//@// #define C1_FreqDecY             vq1844      // Freq. decelerazione asse Y [KHz]


//------------------------------------------------------------------------
// Vq1851 - Vq1900 Tabellone parametri dinamici  - Variabili matrici base
// Matrice di base   Id=102

#define C1_TabSpostamentoMm     vq1851      // Spostamento [mm]
#define C1_TabVelAgoRPM         vq1852      // Vel. ago [RPM]

#define C1_AnticipoX            vq1853      // Anticipo start stop X [gradi]
#define C1_AnticipoY            vq1854      // Anticipo start stop Y [gradi]

#define C1_FrqLavX              vq1855      // Frequenza di lavoro X [KHz]
#define C1_StpAccX              vq1856      // Step di accelerazione X
#define C1_FrqAccX              vq1857      // Frequenza accelerazione X [KHz]
#define C1_StpDecX              vq1858      // Step di decelerazione X
#define C1_FrqDecX              vq1859      // Frequenza decelerazione X [KHz]

#define C1_FrqLavY              vq1860      // Frequenza di lavoro Y [KHz]
#define C1_StpAccY              vq1861      // Step di accelerazione Y
#define C1_FrqAccY              vq1862      // Frequenza accelerazione Y [KHz]
#define C1_StpDecY              vq1863      // Step di decelerazione Y
#define C1_FrqDecY              vq1864      // Frequenza decelerazione Y [KHz]

//------------------------------------------------------------------------
// Vq1901 - Vq1950 Profilo di cucitura UDF - Variabili matrici base e header
// Matrice di base   Id=111
// Matrice di header Id=112
                                            // ### matrice di base ###
#define C1_BaseParam1           vq1901      // Parametro 1
#define C1_BaseParam2           vq1902      // Parametro 2

                                            // ### matrice di header ###
#define C1_QuoHomeX             vq1911      // Quota Home X
#define C1_QuoHomeY             vq1912      // Quota Home Y
#define C1_UdfVelLavRPM         vq1913      // Vel lavoro ago [RPM]
#define C1_UdfPuntiVelIni       vq1914      // Punti iniziali (no fix3)
#define C1_UdfVelIniRPM         vq1915      // Vel iniziale ago [RPM]
#define C1_UdfPuntiVelRall      vq1916      // Punti rallentamento (no fix3)
#define C1_UdfVelRallRPM        vq1917      // Vel rallentamento ago [RPM]
#define C1_Udf_FeedG0           vq1918      // Feed nei movimenti G0 [mm/min] fix3
#define C1_Udf_ValTensione      vq1919      // Valore Tensione Testa 1
#define C1_Udf_20               vq1920
#define C1_Udf_ValEletSopra     vq1921      // Valore Uscita magnete Sopra
#define C1_Udf_ValEletSotto     vq1922      // Valore Uscita magnete Sotto
#define C1_Udf_23               vq1923
#define C1_Udf_24               vq1924
#define C1_Udf_25               vq1925
#define C1_Udf_26               vq1926
#define C1_Udf_27               vq1927
#define C1_Udf_28               vq1928
#define C1_Udf_29               vq1929
#define C1_Udf_30               vq1930

#define C1_FEED_G0_IDX          1918        // [INT] Indice Vq Feed movimento G0


//------------------------------------------------------------------------
// Vq1951 - Vq1999 Variabili di interfaccia con firmware Cucitrice e PLC
// ( c:\cnc\sys\cucitrice.txt )

#define C1_VqTotPntCuci         vq1951      // Punti totali cucitura
#define C1_VqActPntCuci         vq1952      // Punto corrente cucitura
#define C1_VqEncImpCuci         vq1953      // Lettura encoder ago [imp]
#define C1_VqEncMmCuci          vq1954      // Lettura encoder ago [mm]
#define C1_VqRpmAgoCuci         vq1955      // Velocita' ago [RPM]
#define C1_VqActStartCuci       vq1956      // Lettura quota start [gradi] (con anticipo)
#define C1_VqActStopCuci        vq1957      // Lettura quota stop  [gradi] (con anticipo)
#define C1_VqAgoStartCuci       vq1958      // Lettura hw quota start [gradi]
#define C1_VqAgoStopCuci        vq1959      // Lettura hw quota stop  [gradi]
#define C1_VqTotParzPnt         vq1960      // N. punti cucitura parziale
#define C1_VqActParzPnt         vq1961      // Punto corrente cucitura parziale
#define C1_VelFeed              vq1962      // Velocità esecuzione Feed
//------------------------------------------------------------------------
// Vq2001 - Vq2700 Variabili per la cucitrice 2

#define C2_VEL_RIF_AGO          2001
#define C2_VelRifAgo            vq2001      // Velocita' riferimento asse ago

#define C2_IMP_RIF_AGO          2002
#define C2_ImpRifAgo            vq2002      // Impulsi riferimento asse ago

#define C2_MM_RIF_AGO           2003
#define C2_MmRifAgo             vq2003      // Mm riferimento asse ago

#define C2_PT_INI_IDX           2004
#define C2_PtIni                vq2004      // Punti iniziali
#define C2_RpmIni               vq2005      // RPM punti iniziali

#define C2_PT_RALL_IDX          2006
#define C2_PtRall               vq2006      // Punti finali
#define C2_RpmRall              vq2007      // RPM punti finali

#define C2_VelMaxAgoRPM         vq2008      // Vel max RPM AGO

#define C2_CntApritens          vq2009      // Contatore impulsi uscita apritensione
#define C2_CntColtello          vq2010      // Contatore impulsi uscita coltello

#define C2_SIMULA_NPOINT_IDX    2011        // [INT]
#define C2_SimulaNumPoint       vq2011      // Numero di punti simulazione
#define C2_SimulaNumPointVel    vq2012      // Vel [%] simulazione npoint
#define C2_SimulaNumPointMsk    vq2013      // Maschera simulazione npoint

#define C2_SIMULA_CONT_IDX      2015        // [INT]
#define C2_SimulaContVbIdx      vq2015      // Indice Vb
#define C2_SimulaContVel1       vq2016      // Vel [%] simulazione continua
#define C2_SimulaContVel2       vq2017      // Vel [%] simulazione continua
#define C2_SimulaContVel3       vq2018      // Vel [%] simulazione continua
#define C2_SimulaContPt12       vq2019      // N. punti cambio da Vel1 a Vel2
#define C2_SimulaContPt23       vq2020      // N. punti cambio da Vel2 a Vel3
#define C2_SimulaContVbPedale   vq2021      // Indice VB pedale per alta velocita'
#define C2_SimulaContVelPedale  vq2022      // Vel pedale alta velocita'[%] simulazione continua

#define C2_FIRST_PT_IDX         2025        // [INT]
#define C2_FirstPtContext       vq2025      // Contesto UDF per calcolo primo punto
#define C2_FirstPtValid         vq2026      // Flag primo punto valido
#define C2_FirstPt_X            vq2027      // Coordinata X del primo punto
#define C2_FirstPt_Y            vq2028      // Coordinata Y del primo punto
#define C2_FirstPt_C            vq2029      // Coordinata C iniziale

#define C2_GANTRY_INFO_IDX      2030        // [INT]
#define C2_GantryErrAct         vq2030      // Errore istantaneo
#define C2_GantryErrMax         vq2031      // Errore massimo
#define C2_GantryErrReset       vq2032      // Reset errore massimo

#define C2_CALC_BUF_IDX         2035        // [INT]
#define C2_CalcBufContext       vq2035      // Contesto ( dato di input )
#define C2_CalcBufErrCode       vq2036      // Codice di errore
#define C2_CalcBufErrStepNum    vq2037      // N. passo UDF dove e' avventuto l'errore
#define C2_CalcBufErrPar        vq2038      // Parametro aggiuntivo dell'errore

#define C2_WARNING_INFO_IDX     2040        // [INT]
#define C2_WarningFlg           vq2040      // Flag Warning
#define C2_WarningAntXMm        vq2041      // Mm per il calcolo dell'anticipo  X
#define C2_WarningAntXRpm       vq2042      // RPM per il calcolo dell'anticipo X
#define C2_WarningAntXPassoUdf  vq2043      // Passo UDF per il calcolo dell'anticipo X
#define C2_WarningAntYMm        vq2044      // Mm per il calcolo dell'anticipo  Y
#define C2_WarningAntYRpm       vq2045      // RPM per il calcolo dell'anticipo Y
#define C2_WarningAntYPassoUdf  vq2046      // Passo UDF per il calcolo dell'anticipo Y
#define C2_WarningFreqXMm       vq2047      // Mm per il calcolo delle frequenze X
#define C2_WarningFreqXRpm      vq2048      // RPM per il calcolo delle frequenze X
#define C2_WarningFreqXPassoUdf vq2049      // Passo UDF per il calcolo delle frequenze X
#define C2_WarningFreqYMm       vq2050      // Mm per il calcolo delle frequenze Y
#define C2_WarningFreqYRpm      vq2051      // RPM per il calcolo delle frequenze Y
#define C2_WarningFreqYPassoUdf vq2052      // Passo UDF per il calcolo delle frequenze Y
#define C2_CntBloccoFiloINI     vq2053      // Contatore impulsi uscita BloccoFiloINI
#define C2_CntBloccoFiloEND     vq2054      // Contatore impulsi uscita BloccoFiloEND

#define C2_FUN74_IDX            2060        // [INT]
#define C2_Fun74_RetCode        vq2060      // RetCode
#define C2_Fun74_QuoObj         vq2061      // Quota obiettivo
#define C2_Fun74_VelObj         vq2062      // Velocita'
#define C2_Fun74_Future         vq2063      // Future
#define C2_Fun74_Acc            vq2063      // Accelerazione ( polinomio grado 5 )
#define C2_Fun74_Tmov           vq2064      // Tempo di movimento ( polinomio grado 5 )
#define C2_Fun74_Offs           vq2065      // Offset anticipo start ( polinomio grado 5 )

#define C2_FASE_AX_AGO_IDX      2070        // [INT]
#define C2_FaseAxAgo            vq2070      // Fase asse ago

#define C2_FASE_AX_C_IDX        2071        // [INT]
#define C2_FaseAxC              vq2071      // Fase asse C

#define C2_CMD_QUO_ABS_IDX      2075        // [INT]
#define C2_CmdQuoAbsRet         vq2075      // RetCode
#define C2_CmdQuoAbsX           vq2076      // QuoAbs X
#define C2_CmdQuoAbsY           vq2077      // QuoAbs Y
#define C2_CmdQuoAbsC           vq2078      // QuoAbs C

#define C2_RPM_AGO_PROFILO_IDX  2100        // [INT]
#define C2_RpmAgoInProfilo      vq2100      // Rpm ago impostati da istruzione del profile ( Vcd1 )

#define C2_TENSIONE_PROFILO_IDX 2101        // [INT]
#define C2_TensioneInProfilo    vq2101      // tensione impostata da istruzione del profile ( Vcd2 )

#define C2_VelRiduzioneRPM      vq2110      // Ulteriore limite RPM Ago ( #M200710_1GF# )

#define C2_CMD_MOVE_AX_C_IDX    2120        // [INT]
#define C2_CmdMoveAxC           vq2120      // Comando di movimento asse C
#define C2_QuoObjAxC            vq2121      // Quota obiettivo asse C
#define C2_NumPtMoveAxC         vq2122      // Punti di cucitura - movimento asse C
#define C2_RpmMoveAxC           vq2123      // Rpm ago durante il movimento dell'asse C
#define C2_IrqNumMoveAxC        vq2124      // IrqNumber interpretazione movimento dell'asse C

#define C2_CMD_GET_IRQ_CNT_IDX  2127        // [INT]
#define C2_IrqCnt               vq2127      // Contatore Irq ( Fun 281 cmd 63 )

#define C2_MOVE_PLC_AX_C_IDX    2130        // [INT]
#define C2_MovePlcAxCErrCode    vq2130      // Mov. asse C - ErrorCode
#define C2_MovePlcAxCQuoObj     vq2131      // Mov. asse C - Quota obiettivo
#define C2_MovePlcAxCVel        vq2132      // Mov. asse C - Velocita'
#define C2_MovePlcAxCAcc        vq2133      // Mov. asse C - Accelerazione
#define C2_MovePlcAxCTime       vq2134      // Mov. asse C - Tempo di movimento
#define C2_MovePlcAxCAnt        vq2135      // Mov. asse C - Anticipo


//------------------------------------------------------------------------
// Vq2651 - Vq2700 Informazioni di debugger del tabellone dei parametri
#define C2_InfoCntPunti         vq2651      // Contatore punti di cucitura
#define C2_InfoAnticipoMm       vq2652      // Mm per il calcolo dell'anticipo
#define C2_InfoAnticipoRpm      vq2653      // RPM per il calcolo dell'anticipo
#define C2_InfoAnticipoPassoUdf vq2654      // Passo UDF per il calcolo dell'anticipo
#define C2_InfoFreqXMm          vq2655      // Mm per il calcolo delle frequenze X
#define C2_InfoFreqXRpm         vq2656      // RPM per il calcolo delle frequenze X
#define C2_InfoFreqXPassoUdf    vq2657      // Passo UDF per il calcolo delle frequenze X
#define C2_InfoFreqYMm          vq2658      // Mm per il calcolo delle frequenze Y
#define C2_InfoFreqYRpm         vq2659      // RPM per il calcolo delle frequenze Y
#define C2_InfoFreqYPassoUdf    vq2660      // Passo UDF per il calcolo delle frequenze Y


//------------------------------------------------------------------------
// Vq2701 - Vq2850 Parametri cucitrice  - Variabili matrici base
// Matrice di base   Id=201

#define C2_SGL_START_STOP_IDX   2701        // [INT]
#define C2_OFFSET_AGO_TACCA_IDX 2716        // [INT]

#define C2_SogliaStart          vq2701      // Soglia start movimento [gradi]
#define C2_SogliaStop           vq2702      // Soglia stop  movimento [gradi]
#define C2_AgoAlto              vq2703      // Ago alto [gradi]
#define C2_StartApriTens        vq2704      // Start camma apritensione [gradi]
#define C2_StopApriTens         vq2705      // Stop  camma apritensione [gradi]
#define C2_StartColtello        vq2706      // Start camma coltello [gradi]
#define C2_StopColtello         vq2707      // Stop  camma coltello [gradi]
#define C2_TSalitaPiedino       vq2708      // Tempo salita piedino [s]
#define C2_TDiscesaPiedino      vq2709      // Tempo discesa piedino [s]
#define C2_ParVelLavRPM         vq2710      // Vel. lavoro ago [RPM]
#define C2_ParPuntiVelIni       vq2711      // Punti iniziali (no fix3)
#define C2_ParVelIniRPM         vq2712      // Vel iniziale ago [RPM]
#define C2_ParPuntiVelRall      vq2713      // Punti rallentamento (no fix3)
#define C2_ParVelRallRPM        vq2714      // Vel rallentamento ago [RPM]
#define C2_StopAgo              vq2715      // Quota stop dell'ago (prima del movimento ad ago alto)
#define C2_OffsetAgoTacca       vq2716      // Offset di fase tran la quota dell'ago e la tacca di zero
#define C2_Par_FeedG0Reset      vq2717      // Feed nei movimenti G0 per azzeramento o reset [mm/min] fix3
#define C2_StartBloccoFiloINI   vq2718      // Start camma blocco filo inizio cucitura [gradi]
#define C2_StopBloccoFiloINI    vq2719      // Stop camma blocco filo inizio cucitura [gradi]
#define C2_StartBloccoFiloEND   vq2720      // Start camma blocco filo fine cucitura [gradi]
#define C2_StopBloccoFiloEND    vq2721      // Stop camma blocco filo fine cucitura [gradi]
#define C2_ParVelRotazione      vq2722      // Velocita' asse C rotazione [%] fix3 movimento iniziale
#define C2_Par_23               vq2723
#define C2_Par_24               vq2724
#define C2_Par_25               vq2725
#define C2_Par_26               vq2726
#define C2_Par_27               vq2727
#define C2_Par_28               vq2728
#define C2_Par_29               vq2729
#define C2_Par_30               vq2730
#define C2_Par_31               vq2731
#define C2_Par_32               vq2732
#define C2_Par_33               vq2733
#define C2_Par_34               vq2734
#define C2_Par_35               vq2735
#define C2_Par_36               vq2736
#define C2_Par_37               vq2737
#define C2_Par_38               vq2738
#define C2_Par_39               vq2739
#define C2_Par_40               vq2740

// Le variabili seguenti servono per origini, rototraslazioni e fattori di scala
//#define C2_ScaleFactX           vq2821      // Fattore di scala X
//#define C2_ScaleFactY           vq2822      // Fattore di scala Y
//#define C2_ScaleCenterX         vq2823      // Centro di scalatura X
//#define C2_ScaleCenterY         vq2824      // Centro di scalatura Y

//#define C2_RotCenterX           vq2825      // Centro di rotazione X
//#define C2_RotCenterY           vq2826      // Centro di rotazione Y
//#define C2_Rotation             vq2827      // Angolo di rotazione

//#define C2_OriginX              vq2828      // Origine X
//#define C2_OriginY              vq2829      // Origine Y
//------------------

// Le variabili seguenti non servono se si usa il tabellone dei parametri dinamici
// Se non si usa il tabellone, queste variabili vanno inserite nella matrice dei parametri
//@// #define C2_ACC_DEC_X_IDX        2830
//@// #define C2_StepAccX             vq2830      // Step accelerazione asse X [step]
//@// #define C2_StepDecX             vq2831      // Step decelerazione asse X [step]

//@// #define C2_FREQ_X_IDX           2832
//@// #define C2_FreqAccX             vq2832      // Freq. accelerazione asse X [KHz]
//@// #define C2_FreqLavX             vq2833      // Freq. lavoro asse X [KHz]
//@// #define C2_FreqDecX             vq2834      // Freq. decelerazione asse X [KHz]

//@// #define C2_ACC_DEC_Y_IDX        2840
//@// #define C2_StepAccY             vq2840      // Step accelerazione asse Y [step]
//@// #define C2_StepDecY             vq2841      // Step decelerazione asse Y [step]

//@// #define C2_FREQ_Y_IDX           2842
//@// #define C2_FreqAccY             vq2842      // Freq. accelerazione asse Y [KHz]
//@// #define C2_FreqLavY             vq2843      // Freq. lavoro asse Y [KHz]
//@// #define C2_FreqDecY             vq2844      // Freq. decelerazione asse Y [KHz]


//------------------------------------------------------------------------
// Vq2851 - Vq2900 Tabellone parametri dinamici  - Variabili matrici base
// Matrice di base   Id=202

#define C2_TabSpostamentoMm     vq2851      // Spostamento [mm]
#define C2_TabVelAgoRPM         vq2852      // Vel. ago [RPM]

#define C2_AnticipoX            vq2853      // Anticipo start stop X [gradi]
#define C2_AnticipoY            vq2854      // Anticipo start stop Y [gradi]

#define C2_FrqLavX              vq2855      // Frequenza di lavoro X [KHz]
#define C2_StpAccX              vq2856      // Step di accelerazione X
#define C2_FrqAccX              vq2857      // Frequenza accelerazione X [KHz]
#define C2_StpDecX              vq2858      // Step di decelerazione X
#define C2_FrqDecX              vq2859      // Frequenza decelerazione X [KHz]

#define C2_FrqLavY              vq2860      // Frequenza di lavoro Y [KHz]
#define C2_StpAccY              vq2861      // Step di accelerazione Y
#define C2_FrqAccY              vq2862      // Frequenza accelerazione Y [KHz]
#define C2_StpDecY              vq2863      // Step di decelerazione Y
#define C2_FrqDecY              vq2864      // Frequenza decelerazione Y [KHz]

//------------------------------------------------------------------------
// Vq2901 - Vq2950 Profilo di cucitura UDF - Variabili matrici base e header
// Matrice di base   Id=211
// Matrice di header Id=212

                                            // ### matrice di base ###
#define C2_BaseParam1           vq2901      // Parametro 1
#define C2_BaseParam2           vq2902      // Parametro 2

                                            // ### matrice di header ###
#define C2_QuoHomeX             vq2911      // Quota Home X
#define C2_QuoHomeY             vq2912      // Quota Home Y
#define C2_UdfVelLavRPM         vq2913      // Vel lavoro ago [RPM]
#define C2_UdfPuntiVelIni       vq2914      // Punti iniziali (no fix3)
#define C2_UdfVelIniRPM         vq2915      // Vel iniziale ago [RPM]
#define C2_UdfPuntiVelRall      vq2916      // Punti rallentamento (no fix3)
#define C2_UdfVelRallRPM        vq2917      // Vel rallentamento ago [RPM]
#define C2_Udf_FeedG0           vq2918      // Feed nei movimenti G0 [mm/min] fix3
#define C2_Udf_ValTensione      vq2919      // Valore Tensione Testa 1 ( non utilizzato )
#define C2_Udf_20               vq2920
#define C2_Udf_ValEletSopra     vq2921      // Valore Uscita magnete Sopra ( non utilizzato )
#define C2_Udf_ValEletSotto     vq2922      // Valore Uscita magnete Sotto  ( non utilizzato )
#define C2_Udf_23               vq2923
#define C2_Udf_24               vq2924
#define C2_Udf_25               vq2925
#define C2_Udf_26               vq2926
#define C2_Udf_27               vq2927
#define C2_Udf_28               vq2928
#define C2_Udf_29               vq2929
#define C2_Udf_30               vq2930

#define C2_FEED_G0_IDX          2918        // [INT] Indice Vq Feed movimento G0


//------------------------------------------------------------------------
// Vq2951 - Vq2999 Variabili di interfaccia con firmware Cucitrice e PLC
// ( c:\cnc\sys\cucitrice.txt )

#define C2_VqTotPntCuci         vq2951      // Punti totali cucitura
#define C2_VqActPntCuci         vq2952      // Punto corrente cucitura
#define C2_VqEncImpCuci         vq2953      // Lettura encoder ago [imp]
#define C2_VqEncMmCuci          vq2954      // Lettura encoder ago [mm]
#define C2_VqRpmAgoCuci         vq2955      // Velocita' ago [RPM]
#define C2_VqActStartCuci       vq2956      // Lettura quota start [gradi] (con anticipo)
#define C2_VqActStopCuci        vq2957      // Lettura quota stop  [gradi] (con anticipo)
#define C2_VqAgoStartCuci       vq2958      // Lettura hw quota start [gradi]
#define C2_VqAgoStopCuci        vq2959      // Lettura hw quota stop  [gradi]
#define C2_VqTotParzPnt         vq2960      // N. punti cucitura parziale
#define C2_VqActParzPnt         vq2961      // Punto corrente cucitura parziale
#define C2_VelFeed              vq2962      // Velocità esecuzione Feed

