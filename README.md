# electronics-Final-Project

ENTITY Final_Project IS
	PORT (
			segs : OUT BIT_VECTOR (6 DOWNTO 0);
			BIN : IN BIT_VECTOR (4 DOWNTO 0));
END Final_Project;

ARCHITECTURE Behavioral OF Final_Project IS

BEGIN
 
    PROCESS (count) 
 VARIABLE count : INTEGER := 0;
 
	  BEGIN 
	  CASE count IS 
	  
	WHEN 0 => segs <= "0000001";
		   IF BIN = "0000" THEN count := count + 1; 
		ELSE segs <= "1111110"; 
		END IF;
	WHEN 1 => segs <= "1001111";
			IF BIN = "0001" THEN count := count + 1; 
		ELSE segs <= "1111110"; 
		END IF;
	WHEN 2 =>  segs <= "0010010";
			IF BIN = "0001" THEN count := count + 1; 
		ELSE segs <= "1111110"; 
		END IF;
	WHEN 3 => segs <= "0000110";
			IF BIN = "0001" THEN count := count + 1; 
		ELSE segs <= "1111110"; 
		END IF;
	WHEN 4 =>  segs <= "1001100";
			IF BIN = "0001" THEN count := count + 1; 
		ELSE segs <= "1111110"; 
		END IF;
	WHEN 5 => segs <= "0100100";
			IF BIN = "0001" THEN count := count + 1; 
		ELSE segs <= "1111110"; 
		END IF;
	WHEN 6 => segs <= "0100000";
			IF BIN = "0001" THEN count := count + 1; 
		ELSE segs <= "1111110"; 
		END IF;
	WHEN 7 => segs <= "0001101";
			IF BIN = "0001" THEN count := count + 1; 
		ELSE segs <= "1111110"; 
		END IF;
	WHEN 8 => segs <= "0000000";
			IF BIN = "0001" THEN count := count + 1; 
		ELSE segs <= "1111110"; 
		END IF;
	WHEN 9 => segs <= "0000100";
			IF BIN = "0001" THEN count := count + 1; 
		ELSE segs <= "1111110"; 
		END IF;
	WHEN 10 => segs <= "0001000";
			IF BIN = "0001" THEN count := count + 1; 
		ELSE segs <= "1111110"; 
		END IF;
	WHEN 11 => segs <= "1100000";
			IF BIN = "0001" THEN count := count + 1; 
		ELSE segs <= "1111110"; 
		END IF;
	WHEN 12 => segs <= "0110001";
			IF BIN = "0001" THEN count := count + 1; 
		ELSE segs <= "1111110"; 
		END IF;
	WHEN 13 => segs <= "1000010";
			IF BIN = "0001" THEN count := count + 1; 
		ELSE segs <= "1111110"; 
		END IF;
	WHEN 14 => segs <= "0110000";
			IF BIN = "0001" THEN count := count + 1; 
		ELSE segs <= "1111110"; 
		END IF;
	WHEN 15 => segs <= "0110000";
			IF BIN = "0001" THEN count := count + 1; 
		ELSE segs <= "1111110"; 
		END IF;
		
	WHEN OTHERS => segs <= "1111110"; 
	
	
	END CASE; 
END PROCESS; 
		
END ARCHITECTURE;	
		
			
