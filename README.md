    // Current_LSB = Maximum Expected Current / 2^15 = (80mV / 100mΩ) / 2^15 = 0.00002A
    // Cal = 0.04096 / (Current_LSB / R) = 0.04096 / (0.00002A * 0.1R) = 20480
    ina219_calibrationValue = 20480;

    // 1mA = Current_LSB * bits = 20uA * 50
    ina219_currentDivider_mA = 50;
    
    // 1mW = 20 * Power_LSB(mA) = 20 * 0.02mA
    ina219_powerMultiplier_mW = 0.4;
