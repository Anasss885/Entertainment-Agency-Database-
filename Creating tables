create table customers(
customer_ID int,
customer_name varchar(50),
customer_phone_num int,
  constraint cust_id primary key (customer_ID)
);
create table agents(
agent_id int,
assigned_cost int,
constraint ag_id primary key(agent_id)
);

create table entertainers(
entertainer_id int,
entertainer_phone int,
constraint ent_id primary key(entertainer_id)
);


create table members(
members_id int,
members_rate int,
constraint memb_id primary key (members_id)
);

create table engagmnets(
engagment_id int,
category varchar(40),
cus_id int REFERENCES customers(customer_ID),
ag_id int REFERENCES agents(customer_ID),
ent_id int REFERENCES Entertainers(entertainer_id),
constraint eng_id primary key(engagment_id)
);


create table musical_Styles( --this is the only validation table exists
style_id int,
constraint st_id primary key(style_id)
)



--Starting to create linkage tables

create table musical_preferences(
For_Custid int REFERENCES customers(customer_ID),
For_Stid int REFERENCES Musical_Styles(style_id)
);


create table Entertainer_styles(
For_Custid int REFERENCES customers(customer_ID),
For_Stid int REFERENCES Musical_Styles(style_id),
For_entid int REFERENCES Entertainers(entertainer_id)
);


create table Entertainer_members(
For_membid int REFERENCES Members(members_id),
For_entid int REFERENCES Entertainers(entertainer_id)
);




















