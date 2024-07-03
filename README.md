# Floating-Point-Digital-Multiplier-Project
module vedic_multiplier_4bit(
    input [3:0] A, // 4-bit input A
    input [3:0] B, // 4-bit input B
    output [7:0] P // 8-bit output product
);
    wire [3:0] temp0;
    wire [3:0] temp1;
    wire [3:0] temp2;
    wire [3:0] temp3;
    wire [7:0] temp4;
    wire [7:0] temp5;
    wire [7:0] temp6;

    // Partial products
    assign temp0 = A[1:0] * B[1:0];
    assign temp1 = A[3:2] * B[1:0];
    assign temp2 = A[1:0] * B[3:2];
    assign temp3 = A[3:2] * B[3:2];

    // Sum partial products
    assign temp4 = {4'b0, temp0} + {temp1, 2'b0};
    assign temp5 = temp4 + {temp2, 2'b0};
    assign temp6 = {temp3, 4'b0} + temp5;
    // Final product
    assign P = temp6;
endmodule
