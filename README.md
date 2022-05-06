# electronics-Final-Project

ENTITY Final_Project IS
	PORT ( SIGNAL count : INTEGER := 0;
			segs : OUT BIT_VECTOR (6 DOWNTO 0);
			BIN : IN BIT_VECTOR (4 DOWNTO 0));
END Final_Project;

ARCHITECTURE Behavioral OF Final_Project IS

BEGIN

    PROCESS (count) 

	  
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
	WHEN 3 => 
			IF BIN = "0001" THEN count := count + 1; 
		ELSE segs <= "1111110"; 
		END IF;
	WHEN 4 => 
			IF BIN = "0001" THEN count := count + 1; 
		ELSE segs <= "1111110"; 
		END IF;
	WHEN 5 => 
			IF BIN = "0001" THEN count := count + 1; 
		ELSE segs <= "1111110"; 
		END IF;
	WHEN 6 => segs <= "1001111";
			IF BIN = "0001" THEN count := count + 1; 
		ELSE segs <= "1111110"; 
		END IF;
	WHEN 7 => segs <= "1001111";
			IF BIN = "0001" THEN count := count + 1; 
		ELSE segs <= "1111110"; 
		END IF;
	WHEN 8 => segs <= "1001111";
			IF BIN = "0001" THEN count := count + 1; 
		ELSE segs <= "1111110"; 
		END IF;
	WHEN 9 => segs <= "1001111";
			IF BIN = "0001" THEN count := count + 1; 
		ELSE segs <= "1111110"; 
		END IF;
	WHEN 10 => segs <= "1001111";
			IF BIN = "0001" THEN count := count + 1; 
		ELSE segs <= "1111110"; 
		END IF;
	WHEN 11 => segs <= "1001111";
			IF BIN = "0001" THEN count := count + 1; 
		ELSE segs <= "1111110"; 
		END IF;
	WHEN 12 => segs <= "1001111";
			IF BIN = "0001" THEN count := count + 1; 
		ELSE segs <= "1111110"; 
		END IF;
	WHEN 13 => segs <= "1001111";
			IF BIN = "0001" THEN count := count + 1; 
		ELSE segs <= "1111110"; 
		END IF;
	WHEN 14 => segs <= "1001111";
			IF BIN = "0001" THEN count := count + 1; 
		ELSE segs <= "1111110"; 
		END IF;
	WHEN 15 => segs <= "1001111";
			IF BIN = "0001" THEN count := count + 1; 
		ELSE segs <= "1111110"; 
		END IF;
		
	WHEN OTHERS => segs <= "1111110"; 
	
	
	END CASE; 
END PROCESS; 
		
END ARCHITECTURE;	

			--WHEN X"3" => segs <= "0000110";
			--WHEN X"4" => segs <= "1001100";
			--WHEN X"5" => segs <= "0100100";
			--WHEN X"6" => segs <= "0100000";
			--WHEN X"7" => segs <= "0001101";
			--WHEN X"8" => segs <= "0000000";
			--WHEN X"9" => segs <= "0000100";
			--WHEN X"A" => segs <= "0001000";
			--WHEN X"B" => segs <= "1100000";
			--WHEN X"C" => segs <= "0110001";
			--WHEN X"D" => segs <= "1000010";
			--WHEN X"E" => segs <= "0110000";
			--WHEN X"F" => segs <= "0110000";
			--WHEN OTHERS => segs <= "1111110";
			
